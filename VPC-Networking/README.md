# Google Cloud Virtual Private Cloud (VPC) – Networking Fundamentals

##  Objective

Understand and configure **VPC networking** by exploring the default network, creating a new auto mode VPC, adding firewall rules, and testing VM connectivity.

---

##  Tools & Services Used

* VPC Network
* Compute Engine
* Firewall Rules (ICMP, SSH, RDP, Custom)

---

##  Steps Performed

1. Explored the *default VPC network*, subnets, routes, and firewall rules.
2. Deleted the default VPC network and confirmed that VM instances could not be created.
3. Created a new **auto mode VPC network** named "mynetwork" with default firewall rules.
4. Created two VM instances in different regions ("mynet-us-vm" and "mynet-r2-vm").
5. Tested connectivity via SSH and "ping" (internal & external IPs).
6. Removed firewall rules step by step to observe effects on connectivity.

---

##  Key Learnings

* A VPC network is essential for VM creation and connectivity.
* *Firewall rules* directly control SSH and ICMP (ping) access.
* Internal and external IPs behave differently under firewall constraints.
* Default rules (allow-ssh, allow-icmp, allow-rdp, allow-custom) ensure basic connectivity.

---

##  Real-World Application

Understanding VPC fundamentals is critical for **cloud security and architecture**. Proper firewall rules enforce the principle of *least privilege*, reducing exposure while enabling required communication.

---

##  Reflection

This lab highlighted how *networks in Google Cloud are isolated and customizable*. I learned the importance of firewall rule order and specificity, and how removing rules can immediately restrict traffic.
