# `userdel`
deletes a user from the system
## options
* `-r`: deletes all files and subdirectories of the specified user's home directory
## notes
* can only be used by root user or sudoers
* when running this command, no standard output means operation was successful
* when used without `-r` option, it only deletes the user; it does not delete all files and subdirectories of the user's home directory
* deactivating the user's account with `usermod -L` should be considered over `userdel`