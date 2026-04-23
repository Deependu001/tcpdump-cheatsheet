# tcpdump-cheatsheet
A structured guide to TCPDump with essential commands, filters, and examples for analyzing network traffic and building strong packet analysis skills.

# 📡 TCPDump - Packet Capture Tool Notes

## 📌 What is TCPDump?
TCPDump is a command-line packet analyzer used to capture and inspect network traffic in real time.  
It is widely used in cybersecurity, networking, and troubleshooting.

## ⚙️ Basic Syntax
tcpdump [options] [filters]

## 🔍 Common Use Cases
- Capture live network packets
- Analyze suspicious traffic
- Debug network issues
- Monitor protocols like HTTP, DNS, TCP

## 🧪 Basic Commands

# Capture packets on default interface
tcpdump

# Capture packets on a specific interface
tcpdump -i eth0

# Capture only a limited number of packets
tcpdump -c 10

# Disable DNS resolution (faster output)
tcpdump -n

# Show packet contents in ASCII
tcpdump -A

# Show packet contents in HEX and ASCII
tcpdump -XX

# Save capture to a file
tcpdump -w capture.pcap

# Read packets from a file
tcpdump -r capture.pcap

## 🎯 Filters

# Capture only TCP packets
tcpdump tcp

# Capture packets from a specific IP
tcpdump host 192.168.1.1

# Capture packets from a source IP
tcpdump src 192.168.1.1

# Capture packets to a destination IP
tcpdump dst 192.168.1.1

# Capture packets on a specific port
tcpdump port 80

# Combine filters
tcpdump tcp and port 80

## 🧾 Example Output
14:32:10 IP 192.168.1.5.443 > 192.168.1.10.52344: Flags [P.], seq 1:52, ack 1, win 502

## ⚠️ Important Notes
- Requires root privileges
- Can generate large output quickly
- Use filters to reduce noise

## 🛡️ Cybersecurity Relevance
- Network traffic analysis
- Detecting suspicious connections
- Incident response and forensics

## 🚀 This repository will be regularly updated with new concepts, commands, and practical insights as I progress in my cybersecurity learning journey.