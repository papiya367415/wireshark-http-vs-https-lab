
# Wireshark HTTP vs HTTPS Lab

## Objective
The purpose of this lab was to analyze and compare HTTP and HTTPS network traffic using Wireshark inside a Kali Linux virtual machine. The lab focused on understanding how encrypted and unencrypted traffic appears during packet analysis.

---

## Tools Used
- Wireshark
- Kali Linux
- VirtualBox
- Firefox Browser

---

## Skills Practiced
- Packet capturing
- DNS traffic analysis
- TCP handshake analysis
- TLS handshake analysis
- HTTP vs HTTPS comparison
- Follow TCP Stream
- Packet filtering
- Traffic conversation analysis
- TCP reset packet analysis

---

## Filters Used During Analysis

```plaintext
dns
tls
tls.handshake
tcp.flags.syn == 1
tcp.flags.reset == 1
tcp.port == 80
tcp.port == 443
ip.addr == 10.0.2.15
