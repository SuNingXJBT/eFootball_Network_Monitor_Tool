
Telegram group channel: https://t.me/efootballCheaterReport

Telegram group: https://t.me/eFootballxjbt

Donation: https://www.paypal.com/paypalme/tacbin

Feature list:
> Use npcap api to sniff the udp traffic. Only support wired connection.  PS/XBOX players need a router/switch supporting port mirroring. Don't support VPN or proxy.
> 
> If VPN create a RAWIP interface, and wireshark can sniff the traffic, then the tool can either.
> 
> Analyse match mode. show oppoent/server's IP/port/location. Thank @SimplyTheTruth's contribution
> 
> Scan the server to get matches amount on it. If player's ISP blocks such scan activity, modify the filename with 'noscan' in it.
> 
> Packet loss rate is calculated by received messages. It reflects the quality of direction Server->you. Latency of PSP match is from tcping of the server. Latency of P2P match is from STUN message between two players.
> 
> Tcping the server every second during the match. A '.' for a successful try and  'X' for failure. '_' means having received a group of messages.  TCPING reflects the quality of direction You->Server. Consecutive 'XXX' means the direction You->Server is broken. It will be laggy in the game.
> 
> If the loss rate and latency changes a lot, a new line will display.
> 
> Every match will be logged in matchlog.csv file.
> 
> User can run the tool with parameter.  'eFootball_network_monitor_Q143552766.exe 2' means choose the second active network adapter as default.
> 
> colorful dot for different latency, press hh to get detail


Modification history:
20240315
avoid incorrect traffic report
Faster server test results
update iplocation, npcap. 

20231216
Update iplocation, correct some data in-app
Optimize display

20231026
update npcap to 1.78. 
1.76 has critical bug. It must be replaced.
some minor modification


20231008
suport IPV6 ip-area  query
orgnize the files

20231002
upddate ip2location, qqwry database
update npcap to 1.76
support IPV6 p2p match

20230814
update ip2location database
minor fix

20230622
update npcap to 1.75
fix the issue when start the tool during a match.

20230520
Support some VPNs such as Wireguard if they use  RAWIP type vitual adapter.
After the VPN is activated, if wireshark can sniff the traffic on the RAWIP adapter, the tool will also support. Don't accept the match if it shows nothing.

20230517
Optimize display, 
minor fix.

20230424
optimize display. 
20230406
Some ISP block scanning of Google server. If it doesn't work properly, use the other file with 'noscan' . The tool will not scan the server to get current matches.

20230401
Maybe finally resolve the consecutive '_' issue 
optimize display, log to csv file

20230318
Highlight some major info. Thank @SimplyTheTruth's contribution

20230313
Maybe resolve the consecutive '_' issue 

20230220
minor fix about port detecting
20230214
Update iplocation database 

20230212
Antenna bar appears but here is no \'*****Confirming****\'  , that means it's changed to TCP match,don't accept

202302010
minor bug fix 

20230131
Optimize  some display issues 

20230130
English  iparea for non-Chinese system. Thank @SimplyTheTruth's contribution

20030125
bug fix for the local IP judgement
Add document for PS/XBOX user. Use port mirroring and this tool to monitor.  Thank  Mohammed Vorajee's contribution.

200221104
Update: alarm 5 seconds ahead of matchmaking antenna bar's appearance.. so that play have plenty time to decide whether accept or not
Choose dedicated server to secure your  network advantage. Install npcap-1.55 first and then run the eFootball_network_monitor. it will detect the latency between user and konami server in real time
Read  readme.pdf for detail.
