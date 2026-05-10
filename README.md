# 🚀 Cisco Network Analysis Study
**Powered by Packet Tracer & NetworkChuck**

This repository documents my hands-on journey into the world of networking. Using **Cisco Packet Tracer on BOSS Linux**, I am breaking down how data moves across a network, following the "Learn it RIGHT NOW" philosophy.

---

## 📅 Day 1: The "Invisible" Logic (Switches & MAC Tables)
* **The Goal:** Connect devices on the same local network and understand how they "talk" without a router.
* **Key Concept:** Switches are "smart." Unlike hubs, they don't broadcast data to everyone; they listen to hardware addresses and build a map.
* **The Lab:** * Connecting multiple PCs to a **Cisco 2960 Switch**.
    * Mapping hardware addresses using the **MAC Address Table**.
    * **Crucial Command:** `show mac address-table` — Visualizing how the switch binds physical ports to unique hardware IDs.
* **Lesson Learned:** If a switch doesn't know where a MAC address is, it floods the network (ARP). Once it learns the port, the communication becomes a direct "point-to-point" conversation.

---

## 📅 Day 2: The Gateway (Routers, Data Travel & Servers)
* **The Goal:** Route traffic between different subnets and access centralized resources.
* **Key Concept:** Routers are the "Post Offices" of the internet. They don't care about MAC addresses; they care about **IP Addresses** and finding the best path to a destination.
* **The Lab:**
    * Configuring **Default Gateways** on PCs to enable inter-network communication.
    * Setting up a **Server** (HTTP/DNS) and verifying connectivity from a different subnet.
    * Utilizing **Simulation Mode** in Packet Tracer to watch the "Packet" travel Layer-by-Layer through the OSI model.
* **Lesson Learned:** Data travel is a relay race. The Switch handles the "inside" track (Layer 2), while the Router handles the "cross-country" marathon (Layer 3) to deliver data to the correct network.

---

## 🛠️ Environment & Tools
* **OS:** BOSS Linux (Debian-based)
* **Simulation:** Cisco Packet Tracer 8.2.2
* **Credit:** Huge thanks to **[NetworkChuck](https://www.youtube.com/@NetworkChuck)** for the Day 1 and Day 2 tutorials. ☕ + 💻

---

## 📂 How to View These Labs
1. Download the `.pkt` files from this repo.
2. Open them in **Cisco Packet Tracer**.
3. Use **Simulation Mode** to see the PDU headers as they move across the devices.

---