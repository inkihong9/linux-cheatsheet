# `useradd`
adds a user to the system
## options
* `-g`: sets the user's default group (aka primary group)
* `-G`: adds the user to additional groups (aka supplemental or secondary groups)
## examples
### example 1: creating new user `ihong` to group `security_team`
`$ sudo useradd ihong -g security_team`
### example 2: creating new user `ihong` to groups `engineering_team`, `admin`, and `security_team`
`$ sudo useradd ihong -G engineering_team,admin,security_team`
## notes
* can only be used by root user or sudoers
* when running this command, no standard output means operation was successful