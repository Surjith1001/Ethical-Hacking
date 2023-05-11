# Nmap-scans

Features of Nmap
        Find security issues – It warns users against external attackers. Nmap scans the server and finds out the path that hackers might use to attack their server.
        Identify open ports– port scanning of target hosts is very easy with the help of Nmap.
        Detect Vulnerabilities – To detect security vulnerabilities in the network, Nmap is the best choice.
        Host discovery – Live hosts in the network can be discovered using Nmap.
        OS Version Detection – Operating system and version detection are also possible through this network mapper.
        Provide crucial information – Nmap also provides additional information such as devices types, reverse DNS (Domain Name System) names, MAC addresses, and IP addresses of all active hosts.
        
# 1. Scan a Range of IP Address

Aim: To scan the entire IP range

Command: nmap <IP range>

Example: nmap 192.168.1.1(here IP range is separated by a dash )

In our example, Nmap will scan the IP addresses 192.168.1.1

<img src="https://user-images.githubusercontent.com/125909533/236458016-f5ff7ab6-8600-43e4-b3f0-d3a532723699.jpeg"/>


# 2. Port Scanning

Aim: To scan a specific port or entire port range.

Command: nmap -p <numeric value> <IP>

Example: nmap -p 80 192.168.0.1
<table>
        <tr>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236470385-5fcabe62-2d99-4705-b9a9-4b5656dfe9c0.png"/><td/>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236470893-927db392-12e6-4f5f-99d1-27485d17ac27.png"/><td/>
                <td> <img src="https://user-images.githubusercontent.com/125909533/236472282-74a152e8-2b6e-48dc-9b9a-2d7bdba5b2e3.png"/><td/>
        <tr/>
        

<table/>

# 3. TCP Ports Scanning
Aim: To scan all tcp ports. 

Command: nmap -p 1-65535 -T4 -A -v p-<port no> <IP>

Example: nmap -p 1-65535 -T4 -A -v p-80 192.168.0.1
        
 <table>
        <tr>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236478098-792f1c35-fdab-4c37-98ad-3c44f072f4d8.png"/><td/>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236478178-5eb51930-b393-40a6-a802-c4d6daac0c90.png"/><td/>
                <td> <img src="https://user-images.githubusercontent.com/125909533/236478261-390a2e14-82a2-4304-954b-f556b76395cf.png"/><td/>
        <tr/>
        

<table/>       
        
# 4. UDP Ports Scanning
Aim: To scan all tcp ports. 

Command: nmap -sS -sU -T4 -A -v <IP>

Example: nmap -sS -sU -T4 -A -v 192.168.0.1
        
 <table>
        <tr>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236482664-526cdeda-56c4-48d7-a199-798cd79a5829.png"/><td/>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236485871-077e747a-f097-492a-8d30-0f4ce88f85eb.png"/><td/>
                <td> <img src="https://user-images.githubusercontent.com/125909533/236485934-21f4ddd1-b141-487c-9add-a0772e4dbbc9.png"/><td/>
        <tr/>
<table/>   
         
# 5. INTENSE Scanning
Aim: To do intene scan. 

Command: nmap -T4 -A -v <IP>

Example: nmap -T4 -A -v 192.168.0.1
        
 <table>
        <tr>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236489757-feb48cd6-89cc-4430-946b-9054d74d8fb9.png"/><td/>
               <td> <img src="https://user-images.githubusercontent.com/125909533/236489807-f21b94ec-e883-4d33-8a37-eaf6b7d73aef.png"/><td/>
                <td> <img src="https://user-images.githubusercontent.com/125909533/236489172-fdd00296-82ce-427c-8528-0d87ce2a8a4c.png"/><td/>
        <tr/>
<table/> 

