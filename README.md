 🕵️‍♂️ Wireshark Protocol Analysis - Internship Task

## 📅 Task Description:
Capture and analyze network traffic using **Wireshark** on a Windows system. Identify at least **three protocols** and export the packet capture for review.

---

## 🖥️ System Information:
- **Operating System**: Windows 10
- **Tool Used**: Wireshark (Latest Version)
- **Network Interface**: Wi-Fi
- **Capture File**: `capture1.pcap`

---

## ✅ Steps Performed:

### 1. Installed Wireshark
- Downloaded from [https://www.wireshark.org](https://www.wireshark.org)
- Installed with default settings including **Npcap**.

### 2. Started Packet Capture
- Opened Wireshark.
- Selected active network interface (**Wi-Fi**).
- Began live packet capture.

### 3. Generated Network Traffic
- Opened `www.google.com`, `www.wikipedia.org` in browser.
- Ran `ping google.com` in Command Prompt to generate ICMP traffic.

### 4. Stopped the Capture
- After 1 minute, stopped capture using the red square stop button.

### 5. Applied Protocol Filters
- Used the display filter bar to isolate specific protocols:
  - `dns`
  - `http`
  - `tcp`

### 6. Identified 3+ Protocols
#### Protocols found:
- **DNS** – Resolving domain names to IP addresses.
- **HTTP** – Web communication using GET requests.
- **TCP** – Transport layer protocol used by DNS and HTTP.
- (Bonus: **ICMP** for ping, **TLS** for encrypted HTTPS)

### 7. Exported the Capture
- Saved as: `capture1.pcap`
- Format: `.pcapng`

---

## 🔍 Protocol Analysis Summary

| Protocol | Description | Example |
|----------|-------------|---------|
| **DNS** | Domain resolution requests (e.g., google.com) | Query sent to `8.8.8.8` |
| **HTTP** | Web browsing requests (unencrypted) | GET request to `www.wikipedia.org` |
| **TCP** | Reliable data transport | SYN → SYN-ACK → ACK handshake |
| **ICMP** | Ping command (optional) | Echo Request and Reply |
| **TLS** | Encrypted HTTPS communication | TLSv1.2 handshake |

---

## 📸 Screenshots Taken:
1. Wireshark installation complete
2. Interface selected for capture
3. Traffic being generated (ping/browser)
4. Packet capture view after stopping
5. HTTP filter applied
6. DNS filter applied
7. TCP packets (SYN, ACK)
8. Export dialog for `.pcap` file
9. Summary written in Notepad

---

## 📂 Files Included (for submission):
- `capture1.pcap` – Saved packet capture
- Screenshots folder – All key screenshots
- `README.md` – This report

---

## 🧠 Observations:
- DNS queries resolved quickly via Google DNS (`8.8.8.8`)
- HTTP packets were easily readable in plaintext
- TCP ensured reliable transport using handshakes
- ICMP used when pinging external domains
- Most secure sites used TLS encryption
