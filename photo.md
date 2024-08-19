# manipulation de fichiers image
```

for file in *.jpg; do echo "${file/IMG_/}"; done

for file in *.jpg; do mv $file "${file/IMG_/}"; done

exiftool '-FileName<CreateDate' -d '%Y%m%d_%H%M%S.%%e' Lumix

```
