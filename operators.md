# `>` and `>>`
redirects the standard output to a target file
## notes
* difference between `>` and `>>` is that `>` overwrites the existing file with a new standard output, and `>>` appends the standard output to the end of the existing file
* if the specified target file does not exist, it will automatically create it
---
# `|` (piping)
sends the standard output of one command as standard input to another command for further processing
## notes
* general form of redirection in Linux
* can be used for something other than filtering