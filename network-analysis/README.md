# Lab 3: Network Traffic Analysis with Wireshark

## Lab Objectives
- Capture and analyze data packets in real-time using Wireshark on Ubuntu Linux.
- Filter for specific protocols such as **DNS** (name resolution) and **HTTP/TLS** (web traffic).
- Identify network header structures and inspect unencrypted packets.

## Methodology and Applied Filters

1. **Interface Selection (`enp0s3`):** Capture from the local network interface on the virtual machine.
2. **DNS Protocol Filtering:**
- Filter applied: `dns`
- Allows viewing of requests and responses for domain name resolution.
3. **Web Traffic Filtering:**
- Filter applied: `http`
- Inspection of GET/POST requests and data exchange.

## Commands and Preparation
```bash
# Wireshark installation
sudo apt update && sudo apt install wireshark -y

# Execution with capture privileges
sudo wireshark
