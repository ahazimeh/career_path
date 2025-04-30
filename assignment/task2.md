# Networking Exam Answers

## Task 2
### Q1. IP Address Classification
```
150.200.0.1, 203.0.113.8
```

### Q2. ARP Protocol Function
ARP finds the MAC address by broadcasting a request for a given IP.

### Q3. HTTPS Transport Protocol
HTTPS relies on UDP 443 under TLS.

### Q4. Network Device Functions
**Hub:** Broadcasts message to all connected devices in the network

**Switch:** Smarter and sends messages to the specific device

**Router:** Sends data to devices outside the LAN

## Task 3
### Ping Test Results

**From Terminal:**
```
64 bytes from mrs09s07-in-f14.1e100.net (172.217.171.238): icmp_seq=1 ttl=112 time=65.3 ms
64 bytes from mrs09s07-in-f14.1e100.net (172.217.171.238): icmp_seq=2 ttl=112 time=64.1 ms
64 bytes from mrs09s07-in-f14.1e100.net (172.217.171.238): icmp_seq=3 ttl=112 time=74.4 ms
64 bytes from mrs09s07-in-f14.1e100.net (172.217.171.238): icmp_seq=4 ttl=112 time=74.1 ms
64 bytes from mrs09s07-in-f14.1e100.net (172.217.171.238): icmp_seq=5 ttl=112 time=73.1 ms
```

**From Website:**
```
64 bytes from mrs09s07-in-f14.1e100.net (172.217.171.238): icmp_seq=1 ttl=112 time=77.4 ms
64 bytes from mrs09s07-in-f14.1e100.net (172.217.171.238): icmp_seq=2 ttl=112 time=73.8 ms
--- google.com ping statistics ---
2 packets transmitted, 2 received, 0% packet loss, time 1002ms
rtt min/avg/max/mdev = 73.771/75.604/77.437/1.833 ms
```

### Security Vulnerability
Yes, by running the command below you can concatenate another command in the system. You could potentially delete, modify, or view sensitive files on the server.

Example:
```
192.168.191.85 && cat /etc/passwd
```

### Security Fix
You will need to update the `shell` parameter to `False`. With that change, you need to pass the argument for the command as follows:

```python
output = subprocess.check_output(
    #cmd,
    ["ping", "-c", str(count), host],
    shell=False,
    text=True,
    stderr=subprocess.STDOUT,
    timeout=timeout
)
```
