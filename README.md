# Basic Network Scanning with Nmap

## Objective
The objective of this task is to perform network scanning using Nmap and identify open ports and running services.

## Tool Used
- Nmap

## Commands Used

### Basic Scan
```bash
nmap 172.20.10.2
```

### Service Version Detection
```bash
nmap -sV 172.20.10.2
```

### Save Output to File
```bash
nmap -sV 172.20.10.2 > nmap_scan_results.txt
```

---

## Findings

| Port | State | Service | Description |
|------|------|------|------|
| 135 | Open | msrpc | Microsoft Remote Procedure Call |
| 139 | Open | netbios-ssn | Windows file sharing |
| 445 | Open | microsoft-ds | SMB file sharing |

---

## Conclusion
Nmap successfully identified open ports and services running on the target system. Open ports can indicate active services and possible security risks if not properly managed.