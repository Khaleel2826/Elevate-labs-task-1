# Elevate-labs-task-1

-Objective
Using Nmap in Kali Linux to scan the local network and identify open ports on active hosts and using Wireshark to capture and analyze packets during the scan.

-Tools Used
OS: Kali Linux 

Tool: Nmap

Packet Analyzer: Wireshark

-Network Details used
Local IP: 10.0.2.15
Network Range: 10.0.2.0/24

-Files Included
taks1_complete.txt: Combined output of all Nmap scans
taks1_wireshark.pcapng: Wireshark packet capture taken during Nmap scanning

-Commands Used
1. Basic TCP SYN Scan
sudo nmap -sS 10.0.2.0/24
2. TCP SYN Scan with Service Version Detection
sudo nmap -sS -sV 10.0.2.0/24
3. TCP SYN Scan with OS Detection
sudo nmap -sS -O 10.0.2.0/24
4. TCP SYN Scan for Specific Ports (22, 80, 443)
sudo nmap -sS -p 22,80,443 10.0.2.0/24
5. Aggressive Scan (OS detection, version, script scanning, traceroute)
sudo nmap -sS -A 10.0.2.0/24
6.Launch Wireshark to Capture Packets
sudo wireshark
7. Combined Output to Single File
{
  echo "=== Basic SYN Scan ==="
  sudo nmap -sS 10.0.2.0/24

  echo "=== Service Detection ==="
  sudo nmap -sS -sV 10.0.2.0/24

  echo "=== OS Detection ==="
  sudo nmap -sS -O 10.0.2.0/24

  echo "=== Specific Ports ==="
  sudo nmap -sS -p 22,80,443 10.0.2.0/24

  echo "=== Aggressive Scan ==="
  sudo nmap -sS -A 10.0.2.0/24
} > task1_complete.txt


-My Finding
Recognised how to use Nmap to execute various port scans, including aggressive, OS, service, and SYN scans.
discovered how to determine which ports on devices connected to a local network are open, closed, and filtered.
Acquired expertise in deciphering Nmap output and linking shared ports to the appropriate services (e.g., 80 for HTTP, 22 for SSH).
I improved my comprehension of how scanning tools communicate with hosts by using Wireshark to track and examine network traffic in real time.
Enhanced abilities with the Linux terminal, such as command chaining, file redirection, and output organisation for documentation.
Acquired the ability to precisely record cybersecurity procedures and findings in a GitHub repository.
