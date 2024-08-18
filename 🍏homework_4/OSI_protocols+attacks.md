# OSI Model Protocols and Attacks

| Уровень | Протоколы | Атаки |
|---------|-----------|-------|
| 7. Прикладной (Application) | HTTP, FTP, SMTP, DNS, POP3 | Phishing, DOS/DDOS, DNS Spoofing |
| 6. Представления (Presentation) | SSL/TLS, JPEG, MPEG | Man-in-the-Middle, SSL Stripping |
| 5. Сеансовый (Session) | NetBIOS, PPTP, SAP, RPC | Session Hijacking, Man-in-the-Middle |
| 4. Транспортный (Transport) | TCP, UDP, SPX, SCTP | SYN Flood, UDP Flood, TCP Session Hijacking |
| 3. Сетевой (Network) | IP, ICMP, IPSec | IP Spoofing, ICMP/Ping Flood, DNS Amplification, Routing Table Poisoning |
| 2. Канальный (Data Link) | Ethernet, PPP, MAC | MAC Flooding, ARP Spoofing, Switch Spoofing |
| 1. Физический (Physical) | Ethernet (физическая реализация), Wi-Fi (радиоволны), Optical Fiber, USB, DSL | Wiretapping, Noise Injection, Physical Tampering, Jamming, Cable Tapping, USB Spoofing |

## Интересные детали:  
SSL/TLS шифрует данные на уровне представления перед их передачей на транспортный уровень.  
DNS Amplification использует протокол DNS, который работает на прикладном уровне, но сама атака происходит на сетевом уровне.  
Многие атаки могут действовать на разных уровнях, например DOS/DDOS может быть на сетевом (ICMP/Ping Flood), транспортном (IP Fragmentation) и прикладном (HTTP Flood, Slowloris).  
Man-in-the-Middle (MitM) может быть на любом уровне OSI.  
