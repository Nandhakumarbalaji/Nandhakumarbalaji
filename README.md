- 👋 Hi, I’m @Nandhakumarbalaji
- 👀 I’m interested in ...networking 
- 🌱 I’m currently learning ...how to find the server which new installed
- 💞️ I’m looking to collaborate on ...network server
- 📫 How to reach me ...slack

<!---
Nandhakumarbalaji/Nandhakumarbalaji is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
once server is installed is rack find the management ip of the switch and also its which connected port.
login to switch using putty
 find out mac address of the server using the command by issue the command show mac address-table interface which its connected.
 once you find the mac address go to palo alto 
 click on networks --> then click on dhcp ---> then click on view allocation
 find the mac address cross check it
 the you find the ip address of the server.
 ### how to find the impi ip of the server which connected to a switch once server is installedis rack find the management ip of the switch
oob-106#show mac address-table interface gigabitEthernet1/0/29
          Mac Address Table
-------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       --------    -----
   1    3cec.ef2f.7b13    DYNAMIC     Gi1/0/29
Total Mac Addresses for this criterion: 1

then login to palo alto. 
login to network then click on view allocation.
you can find the mac address and impi ip address

then create dns entry in Infoblox.

then also perform iperf both in client and server the server which i tested is public server of iperf.

C:\Users\kesav\Downloads\iperf-3.1.3-win64>cd iperf-3.1.3-win64

C:\Users\kesav\Downloads\iperf-3.1.3-win64\iperf-3.1.3-win64>iperf3.exe -c iperf.he.net -t 10
Connecting to host iperf.he.net, port 5201
[  4] local 2405:201:e00d:11b5:d1b2:3d44:bb1d:1a73 port 62537 connected to 2001:470:0:236::2 port 5201
[ ID] Interval           Transfer     Bandwidth
[  4]   0.00-1.00   sec   256 KBytes  2.09 Mbits/sec
[  4]   1.00-2.01   sec   768 KBytes  6.24 Mbits/sec
[  4]   2.01-3.00   sec   768 KBytes  6.35 Mbits/sec
[  4]   3.00-4.01   sec  1.00 MBytes  8.33 Mbits/sec
[  4]   4.01-5.01   sec  1.25 MBytes  10.4 Mbits/sec
[  4]   5.01-6.00   sec  1.00 MBytes  8.47 Mbits/sec
[  4]   6.00-7.01   sec  1.00 MBytes  8.35 Mbits/sec
[  4]   7.01-8.01   sec   512 KBytes  4.18 Mbits/sec
[  4]   8.01-9.01   sec  1.00 MBytes  8.39 Mbits/sec
[  4]   9.01-10.01  sec  1.25 MBytes  10.5 Mbits/sec
- - - - - - - - - - - - - - - - - - - - - - - - -
[ ID] Interval           Transfer     Bandwidth
[  4]   0.00-10.01  sec  8.75 MBytes  7.33 Mbits/sec                  sender
[  4]   0.00-10.01  sec  8.75 MBytes  7.33 Mbits/sec                  receiver

iperf Done.

 
