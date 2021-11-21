[< Back](../readme.md)


### Copy files or folders
```bash
cp -avr <SRC> <CPY> #verbose output
```

### Delete files or folders
```bash
rm -rv <SRC> #verbose output
```

### Move / Remame files or folders
```bash
mv -v <SRC> <TRG> #verbose output

mv -vf <SRC> <TRG> #force

mv -vn <SRC> <TRG> #no overwrite

mv -vi <SRC> <TRG> #interactive

mv -vu <SRC> <TRG> #update (moves source only if it is newer than the target)
``` 

---

### Get size of file / folder
```bash
du -sh <SRC>
```