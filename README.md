# TechSupportFundamentals
Question 1
Overview: Now that you’re super knowledgeable about security, let's put your newfound know-how to the test. You may find yourself in a tech role someday, where you need to design and influence a culture of security within an organization. This project is your opportunity to practice these important skill sets.
Assignment: In this project, you’ll create a security infrastructure design document for a fictional organization. The security services and tools you describe in the document must be able to meet the needs of the organization. Your work will be evaluated according to how well you met the organization’s requirements.
About the organization: This fictional organization has a small, but growing, employee base, with 50 employees in one small office. The company is an online retailer of the world's finest artisanal, hand-crafted widgets. They've hired you on as a security consultant to help bring their operations into better shape.
Organization requirements: As the security consultant, the company needs you to add security measures to the following systems:
An external website permitting users to browse and purchase widgets
An internal intranet website for employees to use
Secure remote access for engineering employees
Reasonable, basic firewall rules
Wireless coverage in the office
Reasonably secure configurations for laptops
Since this is a retail company that will be handling customer payment data, the organization would like to be extra cautious about privacy. They don't want customer information falling into the hands of an attacker due to malware infections or lost devices.
Engineers will require access to internal websites, along with remote, command-line access to their workstations.
Grading: This is a required assignment for the module. 
What you'll do: You’ll create a security infrastructure design document for a fictional organization. Your plan needs to meet the organization's requirements and the following elements should be incorporated into your plan:
Authentication system
External website security
Internal website security
Remote access solution
Firewall and basic rules recommendations
Wireless security
VLAN configuration recommendations
Laptop security configuration
Application policy recommendations
Security and privacy policy recommendations
Intrusion detection or prevention for systems containing customer data

**Authentication system**
Use a multi-factor RADIUS server. This will require all users to provide two forms of authentication (something you know, something you have) for all corporate systems, this should be then extended to a single sign-on (SSO) as soon as possible.

**External website security**
Using HTTPS at a minimum, implementing a web application firewall and scheduling time to update the web server software.

**Internal website security**
The intranet is only accessible to devices on the company LAN or WAN, ensuring only those people who need permission to access parts of the LAN (for example customer data) have it.

**Remote access solutions**
A VPN for people who need access whilst out of the office, as well as administrators' access to perform fixes from anywhere.

**Firewall and basic rules recommendations**
Implement a solution such as pfsense or similar, to configure firewall rules. It should deny all inbound by default and only allow specific outbound traffic. VLANs can be configured to further segment the network.

**Laptop security configuration**
I recommend these features for new laptops:
biometric scanning. 
TPMv2
secureboot
intel bootguard
GPO Policy for Windows update if using Windows.
Full disk encryption.
Application policy recommendations 
A policy for least privilege application access with regular reviews of access. Ensuring applications have recent security patches.

**Intrusion detection or prevention**
An intrusion detection system (IDS) such as snort, along with regularly reviewing the rules and checking logs.
