###  NMAP NESUS AND OPENVAS
#### port:
	* Lets understand this with an example if we have big apartment (application) and each rooms are application then the room number is the port that helps data go to a particular room .
###  Nmap
	* It is a special tool that helps to find which devices are connected on the network .
	* which ports are open 
	* sp basically it scans whole network 
	* used by attackers to see which ports are open so they can atttack if the port is vulnerable .
	* Syntax: nmap -p(portnumber) 80 -oN file.txt ip address 
	* this means read the port number of this ip and save that thing on the file file.txt 
	* if we want to same in xml format then we can use -oX like this file.xml  for all types -oA for all file types 
	* we have flags in nmap 
	* sS - helps to check if that port is open it establishes three way handshaking and last acknowledgement is rejected we dont establish connection instead we just check if the port is open . syn-> <-sync ack  (if port is closed rej) and last syn is rejected .
	* sV checks the version of service
	* -O os detection 
	* -pn this rejects the ping reply even though the host is offline it still manages to scan the ports are open if its ports are exposed.
	* T4: is the timing template where the value ranges from 0 to 5 ranging from low to high speed.
	* If we remove this -O from the command than we have our report generated of that command in shorter time compared to that when we had that -O
	* If we increase time of scanning T5 than it will give us report generation in short period of time but teh report generetaed is less in content.
	* If we find the port is open than we can check that open is vulnerable or not using a command:->**nmap -sV --script vuln 13.219.53.125 -oN output.txt
	* here sV helps to detect open port plus what is running in that particular port including its version

### Nesus
	* This scans a port or open ports and check if its vulnerable.
####  Keyword:
	* CVE : if a particular vulnerability in a particular website or software named as cve .
	* If we have => suppose wordpress have vulnerability in version 3.1 then we cant convey that message to everyone at once then we take out CVE mention version so that people can patch that (update to new version) 
	* so if before exploiting that problem someone exploits that vulnerability than thats called zero day attack. IT returns CVE.
	* 
	
