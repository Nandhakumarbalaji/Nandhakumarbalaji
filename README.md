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


 
