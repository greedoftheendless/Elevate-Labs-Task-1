# 🔍 Nmap Network Scan Report

This project contains the results and insights from a basic Nmap scan conducted on my local network. The scan aimed to identify active devices, open ports to identify potential security/network risks.

## 🛠️ Steps Followed

1. **Install Nmap**  
   Nmap was installed from the [official website](https://nmap.org/download.html).

2. **Determine Local IP Range**  
   Identified the local subnet (e.g., `192.168.1.0/24`) using:
   ```bash
   ip addr
   ```

3. **Run Nmap TCP SYN Scan**  
   Executed the following command to execute a Syn-Scan on the live and open ports:
   ```bash
   sudo nmap -sS 192.168.1.0/24 -o result.txt 
   ```

4. **Capture Observations**  
   - Listed IP addresses of active devices.
   - Noted open ports and corresponding services.

5. **Packet Analysis (Optional)**  
   Packet capture was optionally analyzed using **Wireshark** to verify Nmap scan behavior and responses.

6. **Service Identification & Risk Analysis**  
   - Researched the purpose of open ports (e.g., 22, 80, 443).
   - Identified common vulnerabilities related to exposed services.

## 📌 Notes

- Ensure proper authorization before scanning any network.
- This scan was conducted on a **private/local** network for educational purposes only.

## Results
  The ports listed were:-
    ssh(secure shell)
    http(website)
    https(website)
    two closed tcp servers

## ⚠️ Security Considerations

- Open ports may expose services to potential attacks.
- Unsecured services (e.g., Telnet, FTP) should be disabled or secured.
