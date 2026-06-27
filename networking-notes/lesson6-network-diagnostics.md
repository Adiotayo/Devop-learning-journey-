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
# Network Troubleshooting Flow Chart

A systematic approach used by DevOps Engineers to diagnose network problems.

-------------------------------------------------------

User says:

"My website is not working."

                │
                ▼
    Is DNS resolving correctly?
                │
        nslookup website.com
                │
      ┌─────────┴─────────┐
      │                   │
     YES                 NO
      │                   │
      ▼                   ▼
 Continue         DNS Problem
                  Check:
                  • DNS record
                  • Route53
                  • Domain
                  • Name Servers

-------------------------------------------------------

                │
                ▼
Can I reach the server?

ping website.com

      │
┌─────┴─────┐
│           │
YES         NO
│           │
▼           ▼
Continue    Check:
             • Internet connection
             • Firewall
             • Server offline
             • ICMP blocked

-------------------------------------------------------

                │
                ▼
Can I reach the service port?

nc -zv website.com 443

or

nc -zv website.com 80

      │
┌─────┴─────┐
│           │
YES         NO
│           │
▼           ▼
Continue    Check:
             • Firewall
             • Security Group
             • NACL
             • Service not listening
             • Wrong Port

-------------------------------------------------------

                │
                ▼
Is the web server responding?

curl -I https://website.com

      │
┌─────┴─────┐
│           │
YES         NO
│           │
▼           ▼
Continue    Check:
             • nginx
             • Apache
             • Application
             • HTTPS configuration

-------------------------------------------------------

                │
                ▼
Interpret HTTP Status Code

200
│
Website OK

301
│
Redirect working

302
│
Temporary redirect

403
│
Permission denied

404
│
Page not found

500
│
Application error

502
│
Bad Gateway

503
│
Service unavailable

504
│
Gateway timeout

-------------------------------------------------------

                │
                ▼
Still failing?

Run

traceroute website.com

                │
                ▼
Find where packets stop

Possible causes

• ISP issue

• Firewall

• Router failure

• Network congestion

• AWS Route Table

• NAT Gateway

• Internet Gateway

-------------------------------------------------------

Server still unreachable?

SSH into server

ssh ubuntu@server-ip

                │
                ▼
Check

systemctl status nginx

systemctl status apache2

systemctl status docker

systemctl status ssh

-------------------------------------------------------

If services are running

Check Logs

journalctl

tail -f

cat

less

-------------------------------------------------------

If services are stopped

Restart service

sudo systemctl restart nginx

or

sudo systemctl restart docker

-------------------------------------------------------

Problem solved.