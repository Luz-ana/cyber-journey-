## domain name system (DNS)
-> it is representation of a website in textual form. Instead of typing ip address for a particular website client gives the corresponding domain name for that website . 
For example: facebook.com no one remembers its ip address .

homepage.facebook.com here we have the hierarchy system where homepage is subdomain facebook is second level domain and .com is top level domain .

## Offensive Security Intro 
Finding the loop holes in the  system and breaking into it using nmap 
gobuster 
->Gobuster is a tool to find hidden files and folders 
->gobuster -u url -w "word.txt"
->here u is the url and w is the search list for a particular word.

## New term :
* Patching : Updating something that may be small update that closes the loop hole . For security purpose.

## Defensive Security:
* Here we learn about the loop holes in our system and patch them preventing other hackers to find that weak spot also protecting the system when something happens .
* We look after the devices that needs to be protected 
* Updating and patching the system: Patching helps to stops the attacker from finding that loop hole and attack . Attackers know the weak spot in the old system and that makes them easier to attack so we must keep on updating the system .
* Using prevention tools like : Firewall, Intrusion Protection System
* Firewall: to stop malicious thing from entering the system 
* Intrusion Prevention System : It contains pattern of attacks and if such pattern matches it stops that action.

To sum up its about protecting the system from the attacks that might occur from the loop holes or weak spots by patching and updating the system regularly and responding quickly if something happens.
###  Tools for defensive security :
* SOC (Security Operation Center)
* DFIR (Digital Forensics and Incident Response)
	
#### SOC :
* It watches over the network , system 24/7 and if it finds something fishy it blocks that action immediately .
* Firstly , it checks if the policy is being violated or not (rules and regulations set )
* Incase the credentials are stolen , SOC checks if its from new device and notifies the user , new location , unusual timing 3AM .
* If the user gets logged in into the system and finds something fishy is happening like copying lots of data or anything suspicious it immediately blocks that person .
#####  Threat Intelligence:
* Finding  possible threats , finding what kinds of attacks are possible in the system .
* Collecting the raw data analyzing what the attacker wants, tactics ,techniques they use .
* By doing so we can immediately find out what kind of attack is happening , how, what are the techniques they use and what are the solutions beforehand.
* Here :
* 1. Internal Source: data collected on your own system
		* through the logs :
		* network log: who logged in what task they did 
		* firewall logs: what activities were blocked
		* antivirus logs: what malicious actions were detected 
* 2. External Source :
		* Cyber forums
		* Bots to go through dark web where attackers sell data actions they perform 
		* social media , news, blogs
 So threat intelligence helps to find what kind of attacks are possible who might be a threat and what are the pattern of such attacks  that info is used by soc who watches over the network 24/7 that looks for such analyzed information .
####  digital forensics and incident response
* Forensics :
	* Firstly forensics means finding out what actually happened when that incident tool place using science . So in real life when some crime occurs and the person who committed that crime is not found we investigate the traces he leaves on that spot hair, footprints and so on and using that we find who the culprit is by solving that puzzle 		 			 
	* Digital Forensics :
		*  we have such person that finds the traces of the attacker known as forensic looking at the logs ,deleted files and activities.
		* Network logs: It checks the network logs checking the data that were send from the system what were send into the system the ip address 
		* The deleted files have traces left . Its not completely wiped out and it only leaves an empty space for other files to be entered into that spot 
		* Live system spying : We can check on the current time (RAM) whats happening because sometimes attacker runs some malware on the temporary memory i.e ram .
		* System logs: Who logged in to the system , updates, errors , updates, which programs were used everything is stored over here .
* Incident Response:
	* Firstly , incident is something that is actually bad that has actually happened like attack., data breaching(stealing) , so on.
	* So incident response is about what to do or how would you respond when such incident happens .
	* 4 steps:
		* 1. Team: firstly create a team that is responsible for analyzing and solving such problems . 
		* 2. Finding problem: Find out what is creating the problem , root, using tools to protect the system , SOC to detect the system 24/7 and find out the when the attack is occurring .
		* 3. Stop and eradicate : when the problem is found then stop the root immediately and stop the thing that's causing the problem .
		* 4. Recover and restore : clean those affected file by removing the traces of malware and restore important file and keep on watching the affected system or the affected file .
* Malware analysis :
	* we know different types of malware like :
		* trojan horse
		* virus
		* ransomware
	* so malware analysis helps to know about such malware by using two methods 
		* 1. static
		* 2. dynamic
		
			* 1.static analysis:
				* we convert the given code that might be harmful into assembly language that contains each steps that that code will perform and we wont run and find out what that code really wants to do . Some obfuscated code might create problem because such codes includes unnecessary lines of code that might be very confusing and we can de-obfuscate or we need to figure which is not important .
			* 2. dynamic analysis :
				* here we run the actual code into a safe environment like sandbox, virtual environment . 
				* this helps us to figure out what such malware might do which might not be clear in static analysis 
				* some of the malware might know that its being run in virtual environment so it might hide its true nature which is one of the challenge .

				


