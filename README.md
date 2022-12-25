<h1 align="center">Replaceit</h1>

<p align="center">
<a href="https://replaceit.codewithshin.com/">Replaceit</a>
</p>

<p align="center">
<a href="https://twitter.com/shinokada" rel="nofollow"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow"><img src="https://img.shields.io/github/license/shinokada/replaceit" alt="License"></a>
</p>

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