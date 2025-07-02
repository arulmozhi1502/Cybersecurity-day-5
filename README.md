# Cybersecurity-day-5

---

## Objective
 - Capture and Analyze Network Traffic Using Wireshark


## Tools Used
 - **Wireshark** – A free and open-source packet analyzer for network troubleshooting and analysis.

## Step-by-Step Procedure

### 1. Install Wireshark
- Download and install Wireshark from the official website.
- During installation, allow the setup to install **Npcap** (packet capture driver) if prompted.

### 2. Select Network Interface
- Launch Wireshark.
- From the start screen, select your active interface:
  - `Wi-Fi` for wireless
  - `Ethernet` for LAN
    
### 3. Start Capturing Packets
- Click the **blue shark fin icon** or double-click the interface to start capturing.
- You’ll see packets being listed in real-time.

### 4. Generate Traffic
- Open a browser and visit websites like:
  - `https://google.com`
  - `https://openai.com`
- Open command prompt/terminal and run:
  ```bash
  ping google.com
  nslookup openai.com
### 5. Stop the Capture
 - After 1–2 minutes of activity, click the red stop button.

### 6. Analyze Captured Packets
 - Use display filters to isolate traffic:
   ~ http – Web browsing traffic
   ~ dns – Domain resolution
   ~ icmp – Ping
   ~ tcp / udp – Transport layer
   ~ tls – Secure HTTPS traffic

### 7. Identify Protocols
 - Look into packet details by clicking individual rows.

 - Expand protocol layers (Ethernet > IP > TCP/UDP > Application Layer) to inspect payload.

 - Note the source/destination IPs, ports, and actions (GET, POST, QUERY, etc.)

### 8. Save Your Capture
 - Go to File > Save As
 - Save the file as "network_capture.pcap"
