# Network-Scanner
This script performs a TCP SYN port scan using raw sockets. It sends SYN packets to target ports and detects open ports by checking for SYN-ACK responses. The script constructs IP and TCP headers, calculates checksums, and scans ports 1-1023 by default. It requires root privileges to run and outputs
TCP SYN Port Scanner
This Python script performs a TCP SYN scan using raw sockets to detect open ports on a target machine. It sends SYN packets to specified ports and identifies open ports by checking for SYN-ACK responses.

# Requirements
Python 3.x
Root/Administrator privileges (raw socket access is required)
Features
Sends SYN packets to ports (default: 1-1023)
Detects open ports based on SYN-ACK responses
Constructs custom IP and TCP headers
Calculates checksum for packet integrity
# How to Use
Clone the repository or download the script.

Modify the IP addresses:

Set the source and destination IP addresses in the script.
Change the source_ip and dest_ip variables in the script as needed.
Run the script:

bash
Copy
sudo python3 port_scanner.py
(Use sudo or run as Administrator since raw socket access is needed.)

View the results:
The script will display which ports are open or closed.

# Example Output

Sent SYN to 10.1.12.173:80

Port 80 is OPEN

Sent SYN to 10.1.12.173:443

Port 443 is OPEN

Open ports: [80, 443]
