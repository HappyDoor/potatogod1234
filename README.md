[# potatogod1234](https://cted.cybbh.io/tech-college/cttsb/cctc/net/Net/
NET-MAIT-25-023

cdp-2
IOS (tm) 1600 Software (C1600-NY-L), Version 11.2(12)P, RELEASE SOFTWARE (fc1)

icmp -4 
windows

fragmented-1
46544
fragmented-2
122
ipv6-1
128
ipv6-2
129
ipv6-3
134
ipv6-4
fa:16:3e:35:21:5a
ipv6-5
beef:4:f00d::
hsrp-1
192.168.0.1
hsrp-2
224.0.0.2
hsrp-3
192.168.0.30
hsrp-4
192.168.0.10
vrrp-1
224.0.0.18
vrrp-2
vrrp192.168.1.254
vrrp-3
3
rip-1
2
rip-2
200.0.1.0,200.0.2.0
rip-3
udp 520
eigrpv4-1
192.168.4.0
eigrpv4-2
88
eigrpv4-3
224.0.0.10
eigrpv6-1
2001:db8:0:400::
eigrpv6-2
ff02::a
eigrp-3
100
ospf-1
89
ospf-2
192.168.170.8
ospf-3
224.0.0.5
bgp-1
3
bgp-2
10.0.0.0,172.16.0.0,192.168.4.0
bgp-3
65210
bgp-4
179






task 2
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------

dhcp-1
192.168.0.1
dhcp-2
192.168.0.10
dhcp-3
3600
dns-1
microsoft.com
dns-2
wikipedia.org
dns-3
hotmail.com
dns-4
etas.com
ftp-1
student10/password10
ftp-2
DO_NOT_LOOK.txt
ftp-3
Schrodinger's Cat
ftp-4
38591:42452
http-1
www.faqs.org
http-2
snippets.cdn.mozilla.net
http-3
https://msn.com/
http-4
twitter.com
smtp-1
virginmedia.com
smtp-2
owadomyi2897@virginmedia.com
smtp-3
sizes
smtp-4
mx.google.com
imap-1
neulingern
imap-2
13
imap-3
Jerry Hammons
pop-1
digitalinvestigator@networksims.com
pop-2
3
pop-3
Edinburgh Napier University
ntp-1
192.168.50.50
ntp-2
Sep 27, 2004
ntp-3
3
ssh-1
172.16.40.10
ssh-2
SSH-2.0-OpenSSH_7.9p1 Debian-10+deb10u2
ssh-3
Diffie-Hellman
ssh-4
1410
ssh-5
7
telnet-1
fake/user
telnet-2
/sbin/ping www.yahoo.com
telnet-3
ls
telnet-4
2579865836
telnet-5
1448
radius-1
John.McGuirk
radius-2
1
radius-3
2
radius-4
11
tacas+-1
192.168.1.5
tacas+-2
59087
tacas+-3
1460
tacas+-4
4128
snmp-1
3
snmp-2
10.0.0.150
snmp-3
2001:470:e5bf:1001:1cc7:73ff:65f5:a2f7
snmp-4
udp 161
TFTP-1
192.168.0.13
tftp-2
rfc1350.txt
tftp-3
49



task 3
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
1. ttl
ip[8]<=64||ip6[7]<=64
2. dont fragment
ip[6]&64==64
3. high port
tcp[0:2]>1024||udp[0:2]>1024
4. udp
ip[9]==0x11||ip6[6]==0x11
5. tcp flags
tcp[13]=0x14||tcp[13]=0x11
6. id 
ip[4:2]=213
7. vlan
ether[12:2]==0x8100
8. dscp
ip[1]&0xfc=0x94
10. traceroute
ip[8]=1&&(ip[9]=0x11||ip[9]=0x01)
11. dns 
udp[0:2]==53||udp[2:2]==53||tcp[0:2]==53||tcp[2:2]==53
12. CLIENT CONNECTIONS
tcp[13]=2
13 OPEN PORTS
tcp[13]=18
14 CLOSED PORTS
tcp[13]=20
15 WELL KNOWN PORTS
tcp[2:2]<=1023||udp[2:2]<=1023
16 HTTP
tcp[2:2]=80||tcp[0:2]=80
17 TELNET
tcp[0:2]=23||tcp[2:2]=23
18 ARP
ether[12:2]=0x0806
VLAN HOPPING
ether[12:4]&0xffff0fff=0x81000001&&ether[16:4]&0xffff0fff=0x8100000a
EVIL BIT
ip[6]&0x80=0x80
URGENT EXFIL
tcp[13]&0x20==0x00&&tcp[18:2]!=0x0000
NULL SCAN
ip[16:4]=0x0a0a0a0a&&tcp[13]=0x00
total chaos 
ip[9]=16)
