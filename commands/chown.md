# `chown`
changes the ownership of a file or directory by user or group
## examples
### example 1: changing user owner of `file.txt` to `ihong`:
`$ sudo chown ihong file.txt`
### example 2: changing group owner of `group_file.txt` to `security_team`:
`$ sudo chown :security_team group_file.txt`
## notes
* group name must follow colon (`:`) when running chown command