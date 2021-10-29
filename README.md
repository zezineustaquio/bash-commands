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

### Get file part name
```sh
~% FILE="example.tar.gz"

~% echo "${FILE%%.*}"
example

~% echo "${FILE%.*}"
example.tar

~% echo "${FILE#*.}"
tar.gz

~% echo "${FILE##*.}"
gz
```
