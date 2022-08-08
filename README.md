# BlockIp
 This script will block or unblock a group of up to 10 ip addresses, or CIDR range on the fly using iptables.

## Notes
Blockip can only be run with root privledges, and should be used with care when blocking a CIDR range over ssh. Otherwise, it could render a server unreachable. The script is only meant to be used on the fly, and not be a permanent solution in terms of blocking ip addresses. For blocking a large range of ip addresses consider the companion applicaton to iptables "ipset."

## Installation
Place the file "blockip" in a directory listed anywhere by the $PATH variable for the root account. To run as sudoer you have to call the file explictly from the directory in which it is located ie sudo ./blockip -b ipaddress 
