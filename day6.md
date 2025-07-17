####  Bridged network :
	* so firstly we have to understand about NAT
	* NETWORK ADDRESS TRANSLATION this is used to provide private IPs to the devices connected over a particular router that has been given public IP .
	* so internet doesnt see the private ips so we are on the safe side as we cant be seen through outer world .
	* So NAT is used to translate that private to the public given to the router and router relays that message to the internet.
	
	* now we have the private ip given to the devices connected to the router through subnetting 
	* router => 192.168.10.0/24 (8 8 8 8 = 32 -24) = 8 for host remaining for network id
	* ips for the private devices start from 192.168.10.0 - 192.168.10.255 ( between this)
	* bridged network is a type of network in which vms are given private ip using DHCP and they can be seen by router or the computer itself can ping that particular vm acting like a separate machine


####  GVM :
	* scans a system and finds what is teh problem in that system and what are the loop holes and helps to fix them before any attacker tries to attack .


#### ssh
	* ssh is used to connect to a particular ip or a domain name 

#### reminder about exfiltration:
	* its the task of getting confidential data secretly without anyone knowing its the task of stealing confidential data


### session and cookie
	* so when i am logged in into a wesite for the first time than it creates session like this is her username or uid to know me next time (in notebook of the server) and server creates a cookie that is a session it to the browser so it  stores cookie into my browser
	* next time when i try to open that website in browser, browser sends cookie (showing membership card)/session id and it matches to that notebook data and says oh this is the person and lets me in without any credentials.
