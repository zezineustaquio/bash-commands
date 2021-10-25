# Bash Commands
Sample of useful bash commands

### Find all files by extension
```sh
find . -iname *.csv
```

### Replace text into file
```sh
sed -i 's/old-text/new-text/g' file.txt
```

### Find files and exec command to replace
```sh
find . -iname *.csv -exec sh -c "sed -i 's/old-text/new-text/g' {}" \;
```
