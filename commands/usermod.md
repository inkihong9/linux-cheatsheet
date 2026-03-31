# `usermod`
modifies existing user accounts
## options
* `-g`: changes the user's default group (aka primary group)
* `-G`: changes the user's supplemental groups (aka secondary groups)
* `-a`: appends the user to an existing group, can only be used with the `-G` option
* `-d`: changes the user's home directory
* `-l`: changes the user's login name
* `-L`: locks the account so the user cannot login
## examples
### example 1: changing the user `ihong`'s primary group to `managers`
`$ sudo usermod -g managers ihong`
### example 2: adding user `ihong` to groups `engineering_team`, `admin`, and `security_team`
`$ sudo usermod ihong -G engineering_team,admin,security_team`
## notes
* can only be used by root user or sudoers
* when running this command, no standard output means operation was successful
* when changing the supplemental group of an existing user without `-a` option, `-G` will **replace** any existing supplemental groups with the groups specified after `usermod`
* using `-a` with `-G` ensures the existing user's supplemental groups include both old and new supplemental groups
* option(s) always follow the `usermod` command