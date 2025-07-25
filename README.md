# 🔐 Red Team Pivoting Lab – Network Segmentation & ACL Evasion (Packet Tracer)

🗓️ **Date:** April 2025  
📍 **Tool:** Cisco Packet Tracer  
🎯 **Focus:** Simulated Red Team lateral movement across segmented networks using ACL bypass techniques

---

🎥 Video Walkthrough  
[▶️ Watch on Google Drive](https://drive.google.com/file/d/1pCSEznhMZSmdej0K9S7oCAp7shkYwAks/view)  
_(If it says "still processing", try again in a few minutes — or download the file below.)_

📦 Also available in this repo: [Download segmentation-lab.mkv](segmentation-lab.mkv)

---

## 🧠 Lab Summary

This lab simulates an attacker pivot scenario through a segmented 3-router network.

- R1 and R3 act as DHCP routers  
- R2 enforces ACLs to block direct communication between some PCs  
- The attacker bypasses ACL restrictions by manipulating ICMP flow paths

---

## 🔧 Key Configurations

- Static routing across all routers  
- DHCP on R1 and R3  
- ACLs applied on R2 interfaces  
- Custom ping paths to test asymmetric blocking

---

## ✅ Proof of Functionality

| Test | Result | What It Proves |
|------|--------|----------------|
| PC1 ➜ PC2 ping | ✅ Success | Routing works |
| PC2 ➜ PC3 ping | ❌ Blocked | ACL active |
| PC1 ➜ PC3 ping | ✅ Success | Bypass worked |
| `show access-lists` | ✅ Hits logged | ACL blocking verified |
| `show ip route` | ✅ Valid | Static routing functional |

---

## 📁 Files Included

- `segmentation-lab.pkt` — Packet Tracer topology  
- `segmentation-lab.mkv` — Silent video walkthrough  
- `proof-of-function.txt` — Observations + test results

---

## 🧠 Skills Demonstrated

- ACL configuration & bypass logic  
- Static routing, subnet management  
- DHCP misdirection & segmentation  
- Lateral movement simulation  
- Threat modeling from Red Team POV

---

## ⚠️ Disclaimer

This lab is strictly for educational purposes.  
It simulates attacker techniques in a safe, ethical environment.
