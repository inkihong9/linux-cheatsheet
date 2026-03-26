# APT
Advanced Package Tool (APT) is a debian-derived package management tool that installs packages via shell
## ensuring APT is installed
`$ apt`
## installing package(s) using APT
`$ sudo apt install package [package-n]`
### example
`$ sudo apt install suricata`
## uninstalling package(s) using APT
`$ sudo apt remove package [package-n]`
### example
`$ sudo apt remove tcpdump`
## listing installed applications
`$ apt list --installed`