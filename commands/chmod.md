# `chmod`
changes permissions on files and directories
## usage (symbolic mode)
`$ chmod permission-grant-revoke-string file-or-directory`
## character meanings
| character | description |
| --------- | ----------- |
| `u` | changes will be made to user permissions |
| `g` | changes will be made to group permissions |
| `o` | changes will be made to other permissions |
| `+` | grant permissions |
| `-` | revoke permissions |
| `=` | assigns permissions |
## examples
### example 1: granting and revoking
`$ chmod g+w,o-r access.txt`
* **grant write** permission to the *group* for `access.txt` file
* **revoke read** permission from *other* users for `access.txt` file
### example 2: granting all permissions to all users on the system 
`$ chmod u+rwx,g+rwx,o+rwx login_sessions.txt`
### example 3: revoke all permissions from all users
`$ chmod u-rwx,g-rwx,o-rwx login_sessions.txt`
### example 4: grant read-only to all users on the system
`$ chmod u=r,g=r,o=r login_sessions.txt`
## notes
* short for "change mode"
* in the 1st argument, `u`, `g` and `o` order does not matter
* assigning `-` **revokes** all permissions (e.g., `chmod g=- file.txt` revokes all permissions from *group*)