# ELEVATE_LABS_TASK1
Cyber Security Internship Task 1 
<br></br> Task 1: Scan Your Local Network for Open Ports <br> </br> Objective: Learn to discover open ports on devices in your local network to understand network exposure. Tools: Nmap (free), Wireshark (optional).
<br> </br>
1 Install Nmap <br></br>
 - Nmap on Kali Linux is usually pre-installed. However, we can check it. If it is missing or not by running following commands: <br>   </br> 
 -nmap --version or nmap –-help                </br>   /* --version To check the installed version of nmap  and --help is nmap commands helpbook.</br>  
- And to ensure it's up to date; you can install or reinstall it by using the following commands:
<br>  </br>
- sudo apt update     or      
- sudo apt install nmap                     </br>    /* apt or aptget for package handling tool so you can install/update/remove nmap by using sudo for root privileges.
<br></br> 2.Find your local IP range (e.g., 192.168.1.0/24). <br></br> 
  - IP discovery using command ip addr show <br></br> 

3.Run:  <br></br> - nmap -sS 192.168.1.0/24 to perform TCP SYN scan. Its a half open scan to avoid detection. <br></br>
4.Note down IP addresses and open ports found. <br></br> 
 - Commands used nmap -Pn 192.168.1.0/24, nmap -sn 192.168.1.0/24  <br></br>
5.Optionally analyze packet capture with Wireshark. <br></br>
 - Analyze packets using filters tcp, tcp.port, tcp.port == 80, dns, http, http2, http3, bttps,ssh, udp.  <br></br>
6.Research common services running on those ports. <br></br> 
- Most common ports and services are:  <br></br> port 21 ftp, 22 ssh, 23 telnet, 53 udp, 80 http, 443 https, 123 udp.  <br></br>
7.Identify potential security risks from open ports.<br></br> - Open vulnerable ports leads to exploitation. <br></br>

Outcome: <br> </br> Basic network reconnaissance skills; understanding network service exposure.  <br></br>
Key Concepts: Port scanning, TCP SYN scan, IP ranges, network reconnaissance, open ports, network security basics

 

