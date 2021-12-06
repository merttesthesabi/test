# test
test
nmap -n -sn 192.0.2.0/24 -oG - | awk '/Up$/{print $2}'


$adsi = [ADSI]"WinNT://workstation1"
$Users = $adsi.Children | where {$_.SchemaClassName -eq 'user'}
$Users | Select Name,Password,Description
