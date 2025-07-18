### Address Resolution Protocol 
	* We know IP address that can represent a network or a particular device connected to a network.
	* When we are connected to a router it uses DHCP to assign us an IP or we can also manually assign our device IP within its range (router) and it remains same but in case of DHCP  it changes .
	* when device A and device B are connected over a network and they want to share data than A sends to B's ip and checks if mac corresponding to that IP exists in that network or not and sends to that device. => THIS IS ADDRESS Resolution.
#### Content Addressable Memory Table (CAM)
	* Initially when there is no communication between the devices connected to teh switched this table is empty 
	* Now suppose device A on port 1 is trying to communicate with Device 2 with certain MAC address on certain Port lets say port no 3 
	* when switch receives this request it writes it down on the cam about the sender A mac address and port on the cam table and when it looks for the port of the destination mac it has no clue because there is no such thing on the cam table .
	* Now what it does is floods that frames to all the ports where devices are connected to the switch than the actual person on port 3 whose mac matches to the mac on th frame which sender was trying to send it responds and in cam table switch places the mac and corresponding port of the destination so next time switch only has to look into the cam table for the port number.
	* Initially it floods the frame and remaining ports ignore that request because its not for them.

####  forwarding decision of switch :
	* this means when the switch receives the packet than it decides where to send it that's the forwarding decision.

#### what happens when we make a search in the internet like example.com how does the reply appear on our screen?
	* in our home we are connected to our router having switch and a dns server that resolves the domain name -> ip address so that will help us search that ip on the internet using router .
	* so inorder to connect to our computer to dns server we have our ip address so switch using arp asks corresponding mac to this ip and we get our ip 
	* then computer ask for the ip of the given example.com
	* then we use this ip in our router that checks on the other network that this ip exits in other network.
	* then in the other side we have the switch thing and finally we use mac to connect to the server and it replies with the page we are searching for.
	** I'm connected to my home router which has a switch and DNS forwarder. When I type a domain (like `example.com`), my device sends an ARP request to get the MAC of the DNS (usually router), then sends a DNS query. Router forwards that to an actual DNS server on the internet, gets back the IP. Then my device sends the request to that IP. The request gets routed through the internet, reaches the destination network, where another switch delivers it to the web server using MAC. The server replies back with the web page.
