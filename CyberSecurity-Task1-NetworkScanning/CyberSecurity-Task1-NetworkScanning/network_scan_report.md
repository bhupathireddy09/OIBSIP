# Network Scanning Report

## Objective

To identify open ports and services running on a target machine using Nmap.

## Tool Used

- Nmap 7.99

## Target IP Address

192.168.1.3

## Command Executed

```bash
nmap -sV 192.168.1.3
```

## Scan Results

| Port | State | Service | Version |
|------|--------|---------|---------|
| 135 | Open | msrpc | Microsoft Windows RPC |
| 139 | Open | netbios-ssn | Microsoft Windows NetBIOS |
| 445 | Open | microsoft-ds | SMB Service |
| 902 | Open | ssl/vmware-auth | VMware Authentication Daemon |
| 912 | Open | vmware-auth | VMware Authentication Daemon |
| 5357 | Open | http | Microsoft HTTPAPI httpd 2.0 |
| 6881 | Open | tcpwrapped | Unknown Service |

## Findings

- Host is active and reachable.
- Multiple Windows networking services are running.
- VMware services are enabled.
- SMB service is available on port 445.
- Several ports are filtered by the firewall.

## Conclusion

The Nmap scan successfully identified open ports and running services on the target machine. Network scanning helps security professionals understand exposed services and evaluate potential security risks.
