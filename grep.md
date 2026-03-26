# `grep`
searches a specified file and returns all lines in the file containing a specified string
## standalone usage
`$ grep string filename`
## example
to search for all lines in the file `updates.txt` containing the word `OS`:

`$ grep OS updates.txt`
## `|` piping usage
`$ some-command-with-std-out | grep string`
## example
to search for all lines in the file `updates.txt` containing the word `OS`:

`$ cat updates.txt | grep OS`