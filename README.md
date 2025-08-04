# 🔍 Nmap Network Scan Report

This project documents the results of a local network port scan performed using **Nmap** and analyzed via **Zenmap (GUI)**. The scan identifies active hosts, open ports, and common services running within the network.

---

## 📌 Objective

To scan the local network and discover:
- Devices connected to the network
- Open TCP ports and corresponding services
- Potential services that may require security attention

---

## 🛠 Tools Used

- [Nmap](https://nmap.org/) - Command-line network scanner
- [Zenmap](https://nmap.org/zenmap/) - GUI for Nmap (used for visual analysis)

---

## 🧪 Scan Details

- **Scan Date**: August 4, 2025
- **Scan Type**: TCP SYN Scan
- **Command Used**:
  ```bash
  nmap -sS 192.168.29.0/24
  ```

- **Scan Range**: 192.168.29.0 to 192.168.29.255 (256 IPs)

---

## 📋 Key Results Summary

| Device IP       | Open Ports          | Notable Services          |
|------------------|---------------------|----------------------------|
| 192.168.29.1     | 80, 443, 1900, 7443, 8080, 8443 | HTTP, HTTPS, UPnP, Proxy |
| 192.168.29.87    | 5357                | WSDAPI                     |
| 192.168.29.157   | 5060 (filtered)     | SIP                        |
| 192.168.29.167   | None                | All ports closed           |
| 192.168.29.248   | None                | All ports closed           |
| 192.168.29.189   | 135, 139, 445, 5357 | SMB, WSDAPI                |

---

## 📁 Files Included

- `nmap_public_report.txt` – Cleaned-up text report for public use
- `README.md` – This file

---

## ⚠️ Disclaimer

This scan was conducted on a **private local network** for **educational purposes only**. Do **not** perform Nmap scans on networks you do not own or do not have permission to analyze.
