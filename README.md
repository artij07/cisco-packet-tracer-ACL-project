# cisco-packet-tracer-ACL-project
Standard Access Control List (ACL) implementation using Cisco Packet Tracer
# Cisco Packet Tracer – Standard ACL Project

## 📌 Project Objective
To implement a **Standard Access Control List (ACL)** that allows only a specific host to access the router while denying all other hosts.

---

## 🛠 Tools Used
- Cisco Packet Tracer
- Router
- PCs
- Standard ACL (Access List 10)

---

## 🧠 Network Configuration
- Network: 192.168.1.0/24
- Allowed Host: 192.168.1.10
- Router Interface: FastEthernet0/0

---

## 🔐 ACL Configuration
```bash
access-list 10 permit host 192.168.1.10
access-list 10 deny any

interface fastEthernet 0/0
ip access-group 10 in
