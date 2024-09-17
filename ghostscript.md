# Ghostscript gs PDF manipulation cheatsheet

## combine PDFs
```{bash}
gs -dNOPAUSE -sDEVICE=pdfwrite -sOUTPUTFILE=foobar.pdf -dBATCH foo.pdf bar.pdf
```

## compress PDF
```{bash}
 gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.5 -dNOPAUSE -dQUIET -dBATCH -dPrinted=false -sOutputFile=foo-compressed.pdf foo.pdf
```
