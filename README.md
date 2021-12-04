# test
test
nmap -n -sn 192.0.2.0/24 -oG - | awk '/Up$/{print $2}'
