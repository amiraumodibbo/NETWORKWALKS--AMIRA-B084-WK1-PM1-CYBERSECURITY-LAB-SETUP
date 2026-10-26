# Building a Virtual Cybersecurity Lab: Kali Linux on VirtualBox

<img width="1918" height="1005" alt="i2" src="https://github.com/user-attachments/assets/93e72640-bbf6-41dc-9a90-83febd84da2e" />

This repository documents the step-by-step process of setting up a secure, isolated cybersecurity environment using Kali Linux and Oracle VM VirtualBox. Establishing this lab environment provides a foundational space for safe penetration testing, network analysis, and security experimentation.

## Technologies Used
* **Hypervisor:** Oracle VM VirtualBox
* **Operating System:** Kali Linux 
* **Networking:** NAT (Network Address Translation) Network
* **Configuration:** Manual IPv4 Addressing

---

##  Step-by-Step Implementation

### 1. Installation & Environment Prep
* **Downloaded Software:** Acquired official, verified binaries for Oracle VM VirtualBox and the pre-built VirtualBox image for Kali Linux.
* **Extraction:** Safely extracted the compressed files to a dedicated local directory to prevent file path issues.
* **Hypervisor Setup:** Successfully installed and initialized VirtualBox on the host machine.

### 2. Virtual Machine Deployment
* **Importing the Image:** Utilized VirtualBox's import appliance feature to load the pre-configured Kali Linux `.ova` file.
* **Resource Allocation:** Confirmed virtual hardware allocations (RAM, CPU cores) matched minimum operating requirements for stability.

### 3. Network Isolation & Configuration
* **NAT Network Setup:** Configured a global NAT Network within VirtualBox preferences to allow the VM to safely access the internet while remaining isolated from the local host network.
* **Manual IP Assignment:** Configured the static IPv4 parameters within the Kali Linux network manager interface, manually assigning:
  * IP Address
  * Subnet Mask
  * Default Gateway
  * DNS Servers

### 4. Backup & Version Control
* **Snapshot Management:** Took a clean baseline snapshot immediately following final configuration. This guarantees a safe point-in-time recovery state in the event of system corruption or experimental failure.
<img width="1913" height="971" alt="i" src="https://github.com/user-attachments/assets/d75aa9a7-5f1e-43d1-b221-e18df27c0a88" />


---

##  Key Takeaways
* Developed a foundational understanding of hypervisors and virtualization concepts.
* Gained practical experience in manually configuring Linux network interfaces and routing.
* Implemented system recovery best practices via virtual machine snapshots.
