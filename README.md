# BlockIp
 This script will block and unblock an IP address or CIDR range on the fly using iptables.

## Notes
This script can only be run with root privledges and if not used with care when blocking a CIDR range over ssh can render a server unreachable. The script is only meant to be used on the fly and not meant to be a permanent solution in terms of blocking ip addresses. For blocking a large range of ip addresses consider using the companion applicaton to iptables "ipset".

## Installation
Place the file "blockip" in a directory listed anywhere by the $PATH variable for the root account. To run as sudoer you have to call the file explictly from the directory in which it is located ie sudo ./blockip -b ipaddress 
