# 🌐 Network Infrastructure Mastery - Day 1

## 📌 Overview
This repository documents my journey in **Cyber Security Engineering**. My first deep dive starts with the foundation of how data moves across a network, focusing on **Layer 2 (Data-Link Layer)**.

---

## 🛠 Technical Concepts Learned

### 1. Layer 2 Intelligence: The Switch
Unlike a Hub, a **Switch** operates at Layer 2 of the OSI model. It is a "smart" device that makes forwarding decisions based on **MAC Addresses** rather than broadcasting data to all ports.

### 2. Switching vs. Hubbing
| Feature | Hub | Switch |
| :--- | :--- | :--- |
| **OSI Layer** | Layer 1 (Physical) | Layer 2 (Data-Link) |
| **Data Delivery** | Broadcast (to everyone) | Unicast (to specific recipient) |
| **Efficiency** | High collisions | Eliminates collisions |



### 3. The CAM Table (Content Addressable Memory)
The **CAM Table** is the "brain" of the switch. It maps physical ports to the hardware (MAC) addresses of connected devices. 
* **Process:** When a frame arrives, the switch looks at the source MAC to build the table and the destination MAC to forward the frame.

---

## 💻 Hands-on Lab Practice
**Tool used:** `Cisco Packet Tracer`

I configured a basic LAN topology and verified the switch's behavior using the Command Line Interface (CLI).

### Key Command:
```bash
# To view the mapping of MAC addresses to physical ports
show mac-address-table