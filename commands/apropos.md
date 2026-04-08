# `apropos`
searches the manual page descriptions for a specified string
## options
* `-a`: allows multiple keywords to filter by
## notes
* useful to get a list of commands with a specific keyword
* for example, if I need to change a password but I don't know what command to use, running command `$ apropos password` outputs a list of commands with the keyword `password` in their man pages
* to filter by multiple keywords, use `-a` option (e.g., `$ apropos -a change password`)