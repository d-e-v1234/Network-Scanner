# Network-Scanner
This script performs a TCP SYN port scan using raw sockets. It sends SYN packets to target ports and detects open ports by checking for SYN-ACK responses. The script constructs IP and TCP headers, calculates checksums, and scans ports 1-1023 by default. It requires root privileges to run and outputs
