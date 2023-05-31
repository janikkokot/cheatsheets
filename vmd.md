loading molecules
=================

```bash
vmd> mol new <file>
vmd> mol addfile <file> [..files] first 1 last -1 step 10
```

representation
==============
add representation
------------------
```bash
vmd> mol addrep <molid>
vmd> mol addrep 0
```
change selection
----------------
```bash
vmd> mol modselect <repid> <molid> <selection>
vmd> mol modselect 0 0 water
vmd> mol modselect 0 0 water within 5 of protein
```
update selection
----------------
```bash
vmd> mol selupdate <repid> <molid> [0|1|off|on|false|true]
vmd> mol selupdate 0 0 true
```

show/hide representation
------------------------
```bash
vmd> mol showrep <repid> <molid> [0|1|off|on|false|true]
vmd> mol showrep 0 0 false
```

smoothing window
----------------
```bash
vmd> mol smoothrep <repid> <molid> <smoothing>
vmd> mol smoothrep 0 0 2
```

change drawing style
--------------------

```bash
vmd> mol modstyle <repid> <molid> <style>
vmd> mol modstyle 0 0 NewCartoon
vmd> mol modstyle 0 0 Solvent
```

animation
=========

```bash
vmd> animate forward
vmd> animate pause
vmd> animate speed 0.00-1.00
```
