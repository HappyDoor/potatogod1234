1.
RED-SCR
2.
1
3.
172.16.101.2
4.
1
5.
22
6.
red-dmz-host-1
ssh -v 172.16.101.2
7.
RED-IPS
ssh -v vyos@172.16.120.9
8.
RED-POP
ssh -X vyos@172.16.120.17
9.
4
show interface
10.
106,110,114,118
show interface
11.
22,80
./scan.sh 
172.16.182
97-126
1-100
12.
1980-1989
wget -r http://172.16.182.110
eog 172.16.182.110/hint-01.png
13.
1984,1989
sudo nmap -sU -p1970-1999 172.16.182.110
14.
which dig
nc -u 172.16.182.110 1984
15.
ip address
nc -u 172.16.182.110 1989
16.
1980,1982,1988,1989
sudo nmap -sS -p1-4000 -T4 172.16.182.110
17.
-s
nc 172.16.182.110 1980
18.
local to remote
nc 172.16.182.110 1982
19.
-sU
nc 172.16.182.110 1988
20.
ipconfig /displaydns
nc 172.16.182.110 1989
21.
22
sudo nmap -sS -p1-4000 -T4 172.16.182.106
22.
red-host-1
ssh -v 172.16.182.106
23.
22
sudo nmap -sS -p1-4000 -T4 172.16.182.114
24.
red-host-3
sudo nmap -sS -p1-4000 -T4 172.16.182.114
25.
22
sudo nmap -sS -p1-4000 -T4 172.16.182.118
26.
red-host-4
ssh -v 172.16.182.118
27.
RED-POP2
./scan.sh
172.16.140
1
6
1-100
ssh -v 172.16.140.5
28.
33,35
scan.sh
29.
22,80
scan.sh
30.
1999-2999
wget -r http://172.16.140.33
eog 172.16.140.33/hint-01.png
31.
2305,2800,2828
sudo nmap -sS -p2000-3001 -T4 172.16.140.33
32.
2000,2011,2200,2250,2999

33.
15
traceroute dash.ent1.pcte.mil
34.
6
dig dtic.mil NS +short
35.
Columbus, OH
nc 172.16.140.33 2828
ICANN lookup
36.
20
37.
admin-dns@valvesoftware.com
chatgpt
38.
DigiCert
chatgpt
39.
Cisco
internet
40.
Wayne Bridges
41.
22
sudo nmap -p1-1023 -T4 172.16.182.118
42.
red-int-dmz2-host-2
ssh -v 172.16.140.35
