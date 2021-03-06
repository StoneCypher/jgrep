# jgrep

Recursive grep.

## Getting Started
Install the module with: `npm install jgrep`

## Examples

Search for something starting from current directory.
```unix
$ jgrep waldo
```

Search for something only in current directory.
```unix
$ jgrep waldo --norecurse
```

Search for something including even hidden dirs (eg: .git, .svn).
```unix
$ jgrep waldo --hidden
```

Search for something excluding some dirs.
```unix
$ jgrep waldo -i node_modules,logs
```

Case insensitive search starting from Foo's home directory.
```unix
$ jgrep waldo -p /Users/foo --nocase
```

Search for all terms (contained in a file) in files with specified extensions.
```unix
$ jgrep /Users/foo/terms.txt -p /Users/foo -e js,.json
```

## License
Copyright (c) 2014 Mustafa Rizvi  
Licensed under the MIT license.
