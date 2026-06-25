# Lesson 6 - Network Diagnostics

## ping

Used to test whether a host is reachable.

Example:

ping google.com

## Command

```bash
nc -zv google.com 443
```

### What does it do?

nc
- Netcat
- Opens TCP/UDP connections.

-z
- Zero-I/O mode.
- Checks whether a port is open without sending data.

-v
- Verbose mode.
- Displays detailed connection information.

google.com
- Destination host.

443
- HTTPS port.

Purpose:
Check whether HTTPS is reachable.