# Basic Nmap Network Scanning

## 🎯 Objective

To practice basic network scanning and understand how attackers identify open ports and services.

---

## 🛠️ Tools & Environment
- Linux OS running in Raspberr Pi 4
- RealVNC Viewer (Windows)
- Nmap
- Home Lab

---

## 🔍 Steps I Did
1️⃣ Identify target  
2️⃣ Run scan  
3️⃣ Analyze results  


---

## 📷 Evidence / Screenshots

![scan]("Screenshot 2026-01-02 230250.png")


---

## 📚 Findings / Results

- By scanning the host i found my own machine's ipv4 and use it as my target
- Found open ports 135, 139, 445 and 5357 
---

## 🎓 What I Learned / 

- During my lab activity, I first used nmap -sn to perform host discovery and identify which devices were active on the network.
  This helped me understand how attackers initially map a network and determine potential targets. After identifying my target machine, I then used nmap -Pn to scan it.
  By disabling host discovery, Nmap proceeded to scan the target even if it did not respond to ping, which simulated how attackers can still attempt to enumerate systems that are blocking ICMP requests.

  Through this process, I gained a better understanding of how reconnaissance works in real-world scenarios and why securing network visibility, managing exposed hosts,
  and configuring firewalls properly are important defensive measures.
  
- While scanning my lab network with Nmap, I learned that exposing unnecessary ports is risky because each open port can serve as a potential entry point for attackers. 
  Even if a service is not actively used, an open port can reveal information about the system, such as running services or software versions, which attackers can exploit. 
  This exercise showed me why it’s important to minimize open ports, disable unused services, and properly configure firewalls to reduce the system’s attack surface.

---

## 🛡️ Ethical Note
This was done **only in legal environments**.
