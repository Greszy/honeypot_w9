# Project 10 - Honeypot

Time spent: **24** hours spent in total

> Objective: Setup a honeypot and provide a working demonstration of its features.

### Required: Overview & Setup

- [x] A basic writeup (250-500 words) on the `README.md` desribing the overall approach, resources/tools used, findings

When it comes to working with honeypots my first decision is to understand what kind of honeypot would like I like to use. Honeypots come in different shapes and sizes. They can mimic different kind kinds of applications. We have [different implementations of honeypots] (https://www.symantec.com/connect/articles/guide-different-kinds-honeypots). Some present vulnerable real applications and collect data through a honeywall about the occurring attacks. Others just emulate vulnerabilities rather than expose a real application. 

For this assignment, I used two Vagrant virtual machines, one that is my target (honeypot) and a server one that runs my admin console for monitoring data collected by the honeypot. I used Modern Honey Network (http://threatstream.github.io/mhn/) that helps you quickly implement and efficiently manage honeypots and provides you with an array of tools to analyze data provided by the honeypots. Through MHN I can track type of attacks, date, time, region where the attack comes from, source IP, destination of the attack and many more. The tool let’s you manage multiple different honeypots at the same time. 


- [ ] A specific, reproducible honeypot setup, ideally automated. There are several possibilities for this:
	- A Vagrantfile or Dockerfile which provisions the honeypot as a VM or container
	- A bash script that installs and configures the honeypot for a specific OS
	- Alternatively, **detailed** notes added to the `README.md` regarding the setup, requirements, features, etc.

### Required: Demonstration

- [ ] A basic writeup of the attack (what offensive tools were used, what specifically was detected by the honeypot)
- [ ] An example of the data captured by the honeypot (example: IDS logs including IP, request paths, alerts triggered)
- [ ] A screen-cap of the attack being conducted
    
### Optional: Features
- Honeypot
	- [ ] HTTPS enabled (self-signed SSL cert)
	- [ ] A web application with both authenticated and unauthenticated footprint
	- [ ] Database back-end
	- [ ] Custom exploits (example: intentionally added SQLI vulnerabilities)
	- [ ] Custom traps (example: modified version of known vulnerability to prevent full exploitation)
	- [ ] Custom IDS alert (example: email sent when footprinting detected)
	- [ ] Custom incident response (example: IDS alert triggers added firewall rule to block an IP)
- Demonstration
	- [ ] Additional attack demos/writeups
	- [ ] Captured malicious payload
	- [ ] Enhanced logging of exploit post-exploit activity (example: attacker-initiated commands captured and logged)
