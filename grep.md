# `grep`
searches a specified file and returns all lines in the file containing a specified string
## standalone usage
`$ grep string filename`
## example 1
to search for all lines in the file `updates.txt` containing the word `OS`:

`$ grep OS updates.txt`
## example 2
when searching for a string with multiple words (e.g., Human Resources), then enclose them in quotes

`$ grep 'Human Resources' some_file.txt`

OR

`$ grep "Human Resources" some_file.txt`
## `|` piping usage
`$ some-command-with-std-out | grep string`
## example
to search for all lines in the file `updates.txt` containing the word `OS`:

`$ cat updates.txt | grep OS`