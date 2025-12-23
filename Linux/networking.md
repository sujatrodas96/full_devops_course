# NETWORKING COMMANDS

ifconfig -- Old IP command
ip addr show -- New IP command
ip link show -- NIC info
hostname -I -- Show IP

ping host -- Connectivity
ping -c 4 host -- Limited ping

curl ifconfig.me -- Public IP
nslookup domain -- DNS
dig domain -- Advanced DNS

traceroute host -- Packet route
tracepath host -- Alternative

netstat -tulnp -- Listening ports (old)
ss -tulnp -- Listening ports (new)

telnet host port -- Check port
nc -zv host port -- Port scan

route -n -- Routing
ip route show -- Routing modern

arp -a -- ARP cache
