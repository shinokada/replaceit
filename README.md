# Replaceit

## Description
This script replaces spaces of file names with underscores as the default.

## Usage

```
replaceit [ -m FROM ] [ -t TO ]  
    -f  FROM (Default: space)
    -t  TO   (Default: _)
    -d  Directory name
    -o  One file replacement. Use quotes if the file has space(s).
    -h  Help
```

## Examples

The default changes from a space to _ of file names .

```
$ replaceit  
```

Change from - to _.
```
$ replaceit -f - -t _
```

Quote the file name when change one file with space(s).
```
$ replaceit -o Downloads/test1.pdf 
$ replaceit -o "Downloads/test 1.pdf"
```

Using a directory
```
$ replaceit -d mydir1
```

Quote the directory name when it has space(s).
```
$ replaceit -d "my dir 1"
```