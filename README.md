# Smart-Network-Surveillance
build an AI-based network surveillance system using Python and Wireshark. The system has analysis capabilities with machine learning algorithms for real-time threat detection and behavioral analysis.
## Core Components
## Packet Capture Layer
Uses Wireshark/TShark to collect raw network traffic data in .pcap or .pcapng formats.
Supports live traffic monitoring via pyshark.LiveCapture() for real-time analysis.

## Data Processing Engine
Pyshark (Python wrapper) parses packets into structured data, extracting metadata like:
Source/destination IPs and ports
Protocol types (HTTP, DNS, ICMP)
Payload sizes and timing data

## AI Analysis Layer
Implements machine learning models to:
Detect anomalies in packet sizes/frequencies using built in frameworks
Identify covert channels via payload pattern recognition
Classify traffic types (e.g., distinguishing video streams from file transfers)

## Visualization & Reporting
Generates interactive dashboards with matplotlib and seaborn for protocol distribution
Maps suspicious IPs geographically using GeoLite2 databases
