# brute-force-attack-recording-using-wazuh

## 1. PING EACH MACHINE TO OTHER MACHINE

### A.Kali Linux (Attacker)
![Kali Linux](foto/ping-honeypot.png)

### b.Honeypot Ubuntu
![Honeypot Ubuntu](foto/ping-honeypot.png)

### B.Wazuh Manager
![Wazuh Manager](foto/ping-wazuh-manager.png)


## 2. BRUTE FORCE ATTACK TEST
USING : hydra -l root -x 4:6:a ssh://192.168.1.100:2222
![Wazuh Manager](foto/brute-force.png)


## 3. WAZUH DASHBOARD DISPLAY
![Wazuh Manager](foto/dashboard.png)


## 4. WIRESHARK DISPLAY
USING : ip.src == 192.168.1.10 && tcp.port == 2222 
![Wazuh Manager](foto/wireshark-ip.src.png)
USING : tcp.flags.syn == 1 and tcp.flags.ack == 0
![Wazuh Manager](foto/wireshark.ip.src.png)
