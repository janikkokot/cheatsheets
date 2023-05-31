# Visual Molecular Dynamics Tcl Cheatsheet
## loading molecules

```python
> mol new <file>
> mol addfile <file> [..files] first 1 last -1 step 10
```

## representation
### add representation
```python
> mol addrep <molid>
```
e.g.
```python
> mol addrep 0
```
### change selection
```python
> mol modselect <repid> <molid> <selection>
```
e.g.
```python
> mol modselect 0 0 water
> mol modselect 0 0 water within 5 of protein
```
### update selection
```python
> mol selupdate <repid> <molid> [0|1|off|on|false|true]
```
e.g.
```python
> mol selupdate 0 0 true
```

### show/hide representation
```python
> mol showrep <repid> <molid> [0|1|off|on|false|true]
```
e.g.
```python
> mol showrep 0 0 false
```

### smoothing window
```python
> mol smoothrep <repid> <molid> <smoothing>
```
e.g.
```python
> mol smoothrep 0 0 2
```

### change drawing style

```python 
> mol modstyle <repid> <molid> <style>
```
e.g.
```python
> mol modstyle 0 0 NewCartoon
> mol modstyle 0 0 Solvent
```

## animation

```python
> animate forward
> animate pause
> animate speed 0.00-1.00
```
