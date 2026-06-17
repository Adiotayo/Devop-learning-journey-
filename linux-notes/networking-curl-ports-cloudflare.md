# Networking Notes: HTTP, HTTPS, Curl, Ports, and Cloudflare

## What I learned today

Today I learned how `curl` helps me test how a website or server responds from the terminal.

Simple meaning:

```text
curl = ask a website/server for a response from the terminal
```

A browser shows a webpage visually, but `curl` shows the raw server response in the terminal.

```text
Browser = displays the page nicely
curl = shows the raw response
```

---

## Curl command

Example command:

```bash
curl -I https://www.barnardos.org.uk/
```

What the syntax means:

```text
curl = send a web request
-I = show only the response headers
https://www.barnardos.org.uk/ = the website I am testing
```

Simple meaning:

```text
Ask the website for response information without downloading the full webpage.
```

---

## HTTP status codes

When I used `curl -I`, I saw HTTP status codes.

Important status codes:

```text
200 = OK / successful response
301 = permanent redirect
302 = temporary redirect
403 = forbidden / blocked
404 = page not found
500 = server-side problem
```

Example:

```text
HTTP/2 200
```

This means:

```text
The website responded successfully.
```

Example:

```text
HTTP/2 302
```

This means:

```text
The website is redirecting me to another address.
```

---

## HTTP vs HTTPS

```text
HTTP = normal web traffic, usually port 80
HTTPS = secure encrypted web traffic, usually port 443
```

Example:

```text
http://example.com = uses HTTP / port 80
https://example.com = uses HTTPS / port 443
```

Simple meaning:

```text
HTTPS is the secure version of HTTP.
```

---

## Ports

A port is like a door into a service on a server.

Simple meaning:

```text
Port = door to a service
```

Common ports:

```text
22 = SSH
53 = DNS
80 = HTTP
443 = HTTPS
```

Example:

```text
IP address = building address
Port = room/door inside the building
```

---

## Cloudflare

Cloudflare can sit in front of a website.

Simple flow:

```text
User/browser
→ Cloudflare
→ real website server
```

Cloudflare can help with:

```text
security
caching
DDoS protection
traffic filtering
redirects
performance
```

If I see:

```text
server: cloudflare
```

it means:

```text
Cloudflare responded in front of the website.
```

---

## Difference between nslookup, ping, traceroute, and curl

```text
nslookup = checks DNS and finds the IP address
ping = checks if the destination replies at network level
traceroute = shows the path traffic takes
curl = checks the website/server response
```

Simple troubleshooting flow:

```bash
nslookup website.com
ping website.com
traceroute website.com
curl -I https://website.com
```

---

## My understanding

I understand that when I visit a website, several things happen:

```text
DNS finds the IP address.
The network routes traffic to the destination.
The correct port is used.
The website/server responds.
Cloudflare may sit in front of the website.
Curl helps me inspect the response.
```

Simple mental model:

```text
Name → DNS → IP address → Route → Server → Port → Response
```
200 = OK / successful response 
301 = permanent redirect 
302 = temporary redirect 
403 = forbidden / blocked 
404 = page not found 
500 = server-side problem