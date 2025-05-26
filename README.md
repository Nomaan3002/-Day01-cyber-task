# -Day01-cyber-task
Elevate Labs Internship Task 1 - Network Port Scanning

## 🔍 Objective
The objective of this task is to scan my local network using Nmap to discover open ports on connected devices and understand potential exposure to services.

## 🛠 Tools Used
- Nmap (with Zenmap GUI)

## 🧪 Steps Followed
1. Installed Nmap from the official website.
2. Found my local IP range using `ipconfig` → IP range: `192.168.1.0/24`.
3. Launched Zenmap and ran the following scan:
4. Waited for the scan to complete and saved the output as `scan_results.txt`.
5. Analyzed the scan results and researched the purpose of open ports.

## 📊 Results Summary

| IP Address       | Open Ports     | Services             |
|------------------|----------------|----------------------|
| `192.168.1.1`     | 443            | HTTPS                |
| `192.168.1.4`     | 2869, 5357     | ICSLAP, WSDAPI       |
| Others (1.3, 1.5, 1.7) | None shown  | All ports closed or ignored |

## ⚠️ Risks & Observations

- **443 (HTTPS)** is safe if using valid certificates.
- **2869 & 5357** are often used in Windows systems for internal services, but can reveal information if not behind a firewall.
- Devices with all ports closed (1.3, 1.5, 1.7) are generally well-secured.

## 📚 Learnings

- Understood how Nmap identifies open ports.
- Gained experience using Zenmap to visually analyze the network.
- Learned about common services that may be unintentionally exposed.
