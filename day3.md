###  Docker
	* Lets get this with an example :
	* If we have and application that runs in my computer with a particular environment but it doesnt run in person B computer because his computer doesnt have necessary tools that is required to run that application 
	* so we have docker . Docker is like a package of everything application requires so it can run in anyone's computer 
	* If a person doesnt have python installed that is req to run the app or have diff os no problem docker creates a mini comp with all its requirements installed in that min computer and runs that application anyways.

####  ping 
	* This is used to check if a particular device is up or down and if its reachable or not 
####  sudo (superuser do )
	* this helps you run command in admin level to bring changes in your system .

####  apt
	* Its a package manager that helps to update , remove and install software.

## Tree
	* home
		* luzana
			* downloads
			* desktop
			* documents
	* inorder to see where we are at the present time we need to use => pwd (present directory 
	* inorder to move one step back we can simply type cd ..
	* inorder to change directory (cd Desktop) 
	*  cd ~ takes use to the home
	* cd or cd /  takes us to the root directory 
	
### nmap to find the open ports and services
	* nmap -sV ip  (determining service/version info)

### standard port fot https is :	
	* 443
###  for http
	* port 80
	* response for http page not found -> 404
### gobuster
	* it is a tool used to find hidden files or hidden folders in a website using particular keyword or the url of the website that are possible file name that may be hidden in the website 
	* gobuster dir -u "url" -w home/desktop/word.txt
	* here dir is used to tell find this file /directory on this url and search this word
	* s we have this -u "example.com" -w "words.txt" -x php,html,
	* http://example.com/admin.html
	* http://example.com/admin.xml
	* http://example.com/admin.php
	* if we dont have a particular wordlist just get seclists installed in your system that contains bunch of words for searching secret dir of files using gobuster

### sql injection:
	* its simply messing with the sql of the database using the input 
	* for example: we have 
	* username => admin'#
	* passowr => jpt
	* this means we had entered as admin and commented the password in the sql as # or -- works as commenting rest of the sql 
	* select * from page where name = 'admin' # password =""this is commented out and we have easy access over the page
	
###  ftp 
	* so when we need to transmit files we use ftp manually we need to connect to the ftp server and fill the credentials and get logged in into it.
	* but sometimes we have username = "anonymous" and password ="" this is called anonymous login.so we can easily login and upload or download anything.

### downloading the file after connection with ftp server
	* get filename.txt
	* bye this closes the connection
	
	* mget *.txt here m is multiples files get whose extension is .txt


### bye
	* this helps to dis connect the connection established





	

		
