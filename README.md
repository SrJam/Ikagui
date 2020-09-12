# Geo-Recon
An OSINT CLI tool desgined to fast track IP Reputation and Geo-locaton look up for Security Analysts.

# Setup
This tool is compactible with:
* Any Linux Operating System (Debian, Ubuntu, CentOS)
* Termux

# Linux Setup
```bash
git clone https://github.com/radioactivetobi/geo-recon.git
cd geo-recon
chmod +x geo-recon.py
pip install -r requirements.txt
```
# Termux Setup
```bash
git clone https://github.com/radioactivetobi/geo-recon.git
cd geo-recon
chmod +x geo-recon.py
pip install -r requirements.txt
```
# Sample Syntax Linux and Termux
```bash
root@kali:~/geo-recon# python geo-recon.py 138.121.128.19

░██████╗░███████╗░█████╗░  ██████╗░███████╗░█████╗░░█████╗░███╗░░██╗
██╔════╝░██╔════╝██╔══██╗  ██╔══██╗██╔════╝██╔══██╗██╔══██╗████╗░██║
██║░░██╗░█████╗░░██║░░██║  ██████╔╝█████╗░░██║░░╚═╝██║░░██║██╔██╗██║
██║░░╚██╗██╔══╝░░██║░░██║  ██╔══██╗██╔══╝░░██║░░██╗██║░░██║██║╚████║
╚██████╔╝███████╗╚█████╔╝  ██║░░██║███████╗╚█████╔╝╚█████╔╝██║░╚███║
░╚═════╝░╚══════╝░╚════╝░  ╚═╝░░╚═╝╚══════╝░╚════╝░░╚════╝░╚═╝░░╚══╝

                         By d3xt3r_182
 Github: https://github.com/radioactivetobi | Twitter: @d3xt3r_182
            Usage: python3 geo-recon.py <IPADDRESS> <OPTION>
            
            Use python3 geo-recon.py -h too see the options
            


[*] Running Geo-location Check Against 138.121.128.19

Country: Brazil
Region: Piaui
City: Teresina
Organization: Itech Telecom
ISP: Itech Telecom

[*] Geo-IP Lookup Complete!!!


[*] Running Reputation Check Against 138.121.128.19

Domain: "redeitechtelecom.com.br"
Hostname: []
Usage Type: "Fixed Line ISP"
Confidence of Abuse: 100
Number Times of Reported: 982
Last Reported: "2020-08-21T16:43:12+00:00"
Whitelisted: false

The IP Address 138.121.128.19 Is Malicious and well known for SSH Bruteforce Attacks

[*] IP Reputation Look up Complete!!!
```


# Things added by Hautly (SrJam):

- Support for python3 and pip3.
- Now Geo-Recon no longer supports python below version 3.0 because it is deprecated, sorry.
- NMAP support with the --nmap or -n option after the IP number.
- Longitudinal latitude correction.
- Organization for the creation of new modules and separate and organized APIs.


# To Do List
* [ OK ] Include Longitude & Latitude For Geo-IP Lookup
* [ OK ] Fix API

