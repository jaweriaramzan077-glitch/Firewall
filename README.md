# Firewall# Firewall

## 1. What is a Firewall?

A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predefined rules.

**Example:** It can allow trusted traffic and block unauthorized connections.

---

## 2. Purpose of Firewall

* Prevent unauthorized access
* Control network traffic
* Block suspicious connections
* Protect systems and networks
* Monitor network activity

---

## 3. How Firewall Works

A firewall checks network traffic against security rules and decides whether to **Allow** or **Block** the traffic.

```text
Internet → Firewall → Internal Network
              ↓
        Allow / Block
```

---

## 4. Types of Firewall

### Packet Filtering Firewall

Checks packets using information such as IP addresses, ports, and protocols.

### Stateful Firewall

Tracks the state of active network connections.

### Stateless Firewall

Checks each packet independently according to predefined rules.

### Proxy Firewall

Acts as an intermediary between the client and the destination server.

### Next-Generation Firewall (NGFW)

Provides advanced traffic inspection and additional security features.

---

## 5. Hardware Firewall

A physical device that protects a network by filtering traffic.

```text
Internet → Firewall → Switch → Computers
```

---

## 6. Software Firewall

A firewall installed on a computer or server to control its network connections.

**Example:** Windows Firewall and Linux firewall tools.

---

## 7. Firewall Rules

Firewall rules determine which traffic is allowed or blocked.

Example:

```text
Port 443 → Allow
Port 23  → Block
```

---

## 8. Common Ports

| Port | Service | Purpose                |
| ---- | ------- | ---------------------- |
| 22   | SSH     | Secure Remote Access   |
| 23   | Telnet  | Remote Access          |
| 53   | DNS     | Domain Name Resolution |
| 80   | HTTP    | Web Traffic            |
| 443  | HTTPS   | Secure Web Traffic     |

---

## 9. Firewall and IP Address

A firewall can use IP addresses to control traffic.

```text
192.168.1.10 → Allow
192.168.1.50 → Block
```

---

## 10. Firewall and ACL

**ACL (Access Control List)** is a set of rules used to allow or deny network traffic.

```text
Allow → Trusted Traffic
Deny  → Unauthorized Traffic
```

---

## 11. Firewall vs Antivirus

| Firewall                  | Antivirus                |
| ------------------------- | ------------------------ |
| Controls network traffic  | Detects malware          |
| Allows/blocks connections | Scans files and programs |
| Network security          | Malware protection       |

---

## 12. Firewall Logging

Firewall logs record network and security events such as:

* Source IP
* Destination IP
* Port
* Protocol
* Allow/Block action

---

## 13. Advantages

* Improves network security
* Controls network access
* Blocks unwanted traffic
* Monitors network activity
* Helps prevent unauthorized access

---

## 14. Limitations

* Cannot stop every cyber attack
* Incorrect configuration can create risks
* Cannot replace other security controls
* Requires regular monitoring and updates

---

## 15. Linux Firewall — UFW

UFW stands for **Uncomplicated Firewall**.

### Check Status

```bash
sudo ufw status
```

### Enable Firewall

```bash
sudo ufw enable
```

### Allow SSH

```bash
sudo ufw allow 22/tcp
```

### Allow HTTPS

```bash
sudo ufw allow 443/tcp
```

### Deny Port

```bash
sudo ufw deny 23/tcp
```

---

## 16. Key Points

* Firewall = Network Traffic Security
* Stateful = Tracks connections
* Stateless = Checks packets individually
* ACL = Access Control Rules
* Port 22 = SSH
* Port 80 = HTTP
* Port 443 = HTTPS
* UFW = Linux firewall management tool

## Conclusion

A firewall is an important cybersecurity component that controls network traffic and helps protect systems from unauthorized access.

