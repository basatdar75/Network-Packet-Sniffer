
# Network Packet Sniffer — Technical Documentation

## 1. Project Architecture

The Network Packet Sniffer is a Python-based desktop application designed to capture, inspect, and analyze network traffic.

The application uses a modular workflow consisting of four primary stages:

### 1.1 Packet Capture
Captures network packets from a selected network interface using Scapy and the available packet capture driver.

### 1.2 Packet Analysis
Extracts relevant information from captured packets, including:
- Source IP address
- Destination IP address
- Protocol type
- Source and destination ports (where applicable)
- Packet information and metadata

### 1.3 Security Detection
Uses predefined detection signatures to identify potentially suspicious network activity, including unusual ICMP traffic, TCP SYN activity, suspicious HTTP keywords, and DNS behavior.

### 1.4 Data Export
Allows captured packet information to be exported into CSV format for further inspection and analysis.

## 2. Application Workflow

Network Interface
        ↓
Packet Capture
        ↓
Packet Analysis
        ↓
Security Detection
        ↓
Graphical Display
        ↓
CSV Export

