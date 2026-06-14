# Networking Basics Lesson 1

## Lesson purpose

This lesson introduces the foundation of computer networking.

The goal is to understand:

```text
what a network is
how computers communicate
what an IP address is
what public and private IP addresses mean
what a router does
what DNS does
what ports are
what HTTP and HTTPS mean
basic networking commands
```

Networking is important for DevOps, cloud, infrastructure, cybersecurity, IT support, and platform engineering because most systems need to communicate over a network.

---

# 1. What is a network?

A network is a group of devices connected together so they can communicate.

Examples of devices on a network:

```text
laptop
phone
server
printer
router
switch
firewall
camera
cloud server
```

Simple meaning:

```text
Network = connected devices that can talk to each other
```

Example:

At home, my laptop, phone, smart TV, and router are all part of my home network.

In a company, laptops, servers, printers, switches, firewalls, and cloud systems are connected through networks.

---

# 2. Why do we need networks?

We need networks so devices can share information.

Examples:

```text
My laptop opens a website
My phone sends a WhatsApp message
A server sends data to an application
A user logs into a company system
A cloud app connects to a database
A DevOps engineer connects to a Linux server using SSH
```

Simple meaning:

```text
Networking allows devices and systems to communicate.
```

Without networking, computers would be isolated.

---

# 3. What is the internet?

The internet is a massive global network of connected networks.

Simple meaning:

```text
Internet = many networks around the world connected together
```

My home network is small.

A company network is bigger.

The internet connects many networks globally.

When I visit a website, my laptop sends a request through my router, then through my internet provider, then across the internet to the server hosting the website.

---

# 4. What is a server?

A server is a computer that provides a service to other computers.

Examples:

```text
web server
database server
email server
file server
DNS server
application server
```

Simple meaning:

```text
Server = computer that provides something to other computers
```

Example:

When I visit:

```text
google.com
```

my laptop is asking Google’s servers to send back the web page.

---

# 5. What is a client?

A client is the device or application asking for a service.

Examples:

```text
my laptop
my phone
my browser
an app on my phone
```

Simple meaning:

```text
Client = device or program requesting something from a server
```

Example:

If I open Chrome and visit a website:

```text
Chrome/my laptop = client
Website computer = server
```

---

# 6. Client-server relationship

Most network communication works like this:

```text
Client sends request
Server sends response
```

Example:

```text
I type google.com into my browser
My browser sends a request
Google server receives the request
Google server sends back the web page
My browser displays the page
```

Simple meaning:

```text
Client asks, server responds.
```

---

# 7. What is an IP address?

An IP address is a number used to identify a device on a network.

Simple meaning:

```text
IP address = network address of a device
```

Example IP address:

```text
192.168.1.10
```

Another example:

```text
8.8.8.8
```

A device needs an IP address so other devices know where to send data.

Real-life comparison:

```text
Home address = where a person lives
IP address = where a device is located on a network
```

---

# 8. IPv4

The common IP address format I am learning first is IPv4.

Example:

```text
192.168.1.10
```

IPv4 has four sections separated by dots.

Each section is called an octet.

Example breakdown:

```text
192 = first octet
168 = second octet
1 = third octet
10 = fourth octet
```

Simple meaning:

```text
IPv4 = IP address with four number sections
```

---

# 9. Private IP address

A private IP address is used inside a local network, like a home or office network.

Examples of private IP ranges:

```text
192.168.x.x
10.x.x.x
172.16.x.x to 172.31.x.x
```

Example:

```text
192.168.1.25
```

Simple meaning:

```text
Private IP = address used inside a local network
```

My laptop at home may have a private IP address like:

```text
192.168.1.20
```

This address is useful inside my home network, but it is not normally used directly on the public internet.

---

# 10. Public IP address

A public IP address is used on the internet.

Simple meaning:

```text
Public IP = address visible/reachable on the internet
```

Your home router usually has one public IP address from your internet provider.

Inside the home, devices have private IP addresses.

Outside the home, the internet sees the router’s public IP address.

Simple comparison:

```text
Private IP = inside the house
Public IP = address seen by the outside world
```

---

# 11. Private IP vs public IP

## Private IP

```text
Used inside local networks
Examples: 192.168.1.10, 10.0.0.5
Not directly reachable from the internet
Usually assigned by a router
```

## Public IP

```text
Used on the internet
Assigned by an internet provider or cloud provider
Can identify a network or server on the internet
```

Simple meaning:

```text
Private IP = internal network address
Public IP = internet-facing address
```

---

# 12. What is a router?

A router is a device that connects different networks together.

Simple meaning:

```text
Router = device that forwards traffic between networks
```

At home, your router connects:

```text
your home network
to the internet
```

In a company, routers may connect:

```text
office networks
data centres
cloud networks
branches
internet connections
```

The router helps decide where network traffic should go.

---

# 13. What is a switch?

A switch connects devices inside the same local network.

Simple meaning:

```text
Switch = connects devices inside the same network
```

Example in an office:

```text
laptop
printer
desktop
server
```

These can connect to a switch.

The switch helps devices inside the same local network communicate.

Simple difference:

```text
Switch = connects devices inside one network
Router = connects different networks together
```

---

# 14. What is a firewall?

A firewall controls what network traffic is allowed or blocked.

Simple meaning:

```text
Firewall = security gate for network traffic
```

A firewall can allow or block traffic based on things like:

```text
source IP
destination IP
port number
protocol
application
direction of traffic
```

Example:

A company may allow:

```text
users to access a website on port 443
```

but block:

```text
unknown traffic from the internet into internal servers
```

---

# 15. What is DNS?

DNS means Domain Name System.

DNS translates website names into IP addresses.

Simple meaning:

```text
DNS = phonebook of the internet
```

Humans remember names like:

```text
google.com
```

Computers communicate using IP addresses like:

```text
142.250.x.x
```

So DNS helps translate:

```text
google.com -> IP address
```

Real-life comparison:

```text
Contact name on phone = google.com
Phone number = IP address
```

I remember the name. The phone knows the number.

---

# 16. Why DNS matters

Without DNS, I would need to remember IP addresses for websites.

Instead of typing:

```text
google.com
```

I would need to type an IP address.

Simple meaning:

```text
DNS makes the internet easier for humans to use.
```

In DevOps and cloud, DNS is very important because applications often depend on domain names, load balancers, APIs, and servers resolving correctly.

---

# 17. What is a port?

A port is a number that identifies a specific service on a device.

Simple meaning:

```text
Port = door to a service on a computer
```

A server can run many services at once.

Example:

```text
web service
SSH service
database service
email service
```

Ports help the computer know which service the traffic should go to.

---

# 18. Common ports

Some common ports:

```text
22 = SSH
53 = DNS
80 = HTTP
443 = HTTPS
3306 = MySQL
5432 = PostgreSQL
```

Simple meaning:

```text
Different services listen on different port numbers.
```

Example:

If I connect to a Linux server using SSH, I often use:

```text
port 22
```

If I open a secure website, it usually uses:

```text
port 443
```

---

# 19. What is HTTP?

HTTP means HyperText Transfer Protocol.

HTTP is used for loading websites.

Simple meaning:

```text
HTTP = protocol for web traffic
```

HTTP usually uses:

```text
port 80
```

Example:

```text
http://example.com
```

HTTP is not encrypted by default.

---

# 20. What is HTTPS?

HTTPS is the secure version of HTTP.

Simple meaning:

```text
HTTPS = secure web traffic
```

HTTPS usually uses:

```text
port 443
```

Example:

```text
https://example.com
```

HTTPS encrypts communication between the browser and the website.

Simple difference:

```text
HTTP = normal web traffic, not encrypted
HTTPS = secure encrypted web traffic
```

---

# 21. What is a protocol?

A protocol is a set of rules for communication.

Simple meaning:

```text
Protocol = rules for how devices communicate
```

Examples:

```text
HTTP
HTTPS
SSH
DNS
TCP
UDP
ICMP
```

Each protocol has a purpose.

Example:

```text
HTTP/HTTPS = web traffic
SSH = remote login to servers
DNS = name to IP lookup
ICMP = ping testing
```

---

# 22. What is ping?

`ping` is a command used to test whether another device or website is reachable.

Example:

```bash
ping google.com
```

What the syntax means:

```text
ping = test reachability
google.com = destination I want to test
```

Simple meaning:

```text
Check if my computer can reach google.com.
```

Ping sends small test packets and waits for replies.

If replies come back, the destination is reachable.

To stop ping on Mac/Linux:

```text
Control + C
```

---

# 23. What is traceroute?

`traceroute` shows the path network traffic takes to reach a destination.

Example:

```bash
traceroute google.com
```

What the syntax means:

```text
traceroute = show network path
google.com = destination
```

Simple meaning:

```text
Show the route my traffic takes to reach google.com.
```

This can show the different routers or hops between my computer and the destination.

---

# 24. What is nslookup?

`nslookup` checks DNS information.

Example:

```bash
nslookup google.com
```

What the syntax means:

```text
nslookup = name server lookup
google.com = domain name I want to check
```

Simple meaning:

```text
Ask DNS what IP address belongs to google.com.
```

This helps me see whether DNS is working.

---

# 25. What is curl?

`curl` is a command used to make requests to websites, APIs, or servers.

Example:

```bash
curl https://example.com
```

What the syntax means:

```text
curl = make a web request from the terminal
https://example.com = website I want to request
```

Simple meaning:

```text
Ask a website/server to send back a response.
```

In DevOps, `curl` is very useful for testing:

```text
websites
APIs
health checks
server responses
HTTP status
```

---

# 26. Basic networking commands for today

## ping

```bash
ping google.com
```

Simple meaning:

```text
Check if google.com is reachable.
```

Stop it with:

```text
Control + C
```

---

## traceroute

```bash
traceroute google.com
```

Simple meaning:

```text
Show the network path to google.com.
```

---

## nslookup

```bash
nslookup google.com
```

Simple meaning:

```text
Check the IP address DNS gives for google.com.
```

---

## curl

```bash
curl https://example.com
```

Simple meaning:

```text
Request a webpage from the terminal.
```

---

# 27. Simple communication example

When I visit:

```text
https://google.com
```

this is a simplified version of what happens:

```text
1. My browser asks DNS for google.com.
2. DNS returns an IP address.
3. My laptop sends traffic toward that IP address.
4. My router forwards the traffic to the internet.
5. The traffic reaches Google’s server.
6. Google’s server responds.
7. My browser displays the page.
```

Simple meaning:

```text
DNS finds the address.
Routing moves the traffic.
Ports identify the service.
HTTP/HTTPS controls the web communication.
```

---

# 28. My understanding

A network is a group of connected devices.

The internet is a global network of networks.

An IP address identifies a device on a network.

A private IP is used inside a local network.

A public IP is used on the internet.

A router connects networks.

A switch connects devices inside a local network.

A firewall controls allowed and blocked traffic.

DNS changes names like `google.com` into IP addresses.

Ports identify services on a device.

HTTP and HTTPS are used for websites.

Ping tests reachability.

Traceroute shows the network path.

Nslookup checks DNS.

Curl sends web requests from the terminal.
