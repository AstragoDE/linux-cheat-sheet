[< Back](../readme.md)


## Copy files or folders
```bash
cp -vr <SRC> <CPY> #verbose output
```

## Delete files or folders
```bash
rm -rfv <SRC> #verbose output, force (f)
```

### Delete all files or folders in a directory
```bash
rm -rfv * #verbose output, force (f)
```

## Move / Remame files or folders
```bash
mv -v <SRC> <TRG> #verbose output

mv -vf <SRC> <TRG> #force

mv -vn <SRC> <TRG> #no overwrite

mv -vi <SRC> <TRG> #interactive

mv -vu <SRC> <TRG> #update (moves source only if it is newer than the target)
``` 

## Create folder
```bash
mkdir <NAME>
```

---

## Get size of file / folder
```bash
du -sh <SRC>
```
