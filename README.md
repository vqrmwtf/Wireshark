# Wireshark Network Traffic Analysis: HTTP vs HTTPS

## Project Summary
This project analyzes differences in HTTP and HTTPS traffic using Wireshark in a virtualized Kali Linux environment.

## Environment
- Kali Linux on VirtualBox
- Wireshark v4.x
- Internet connection via bridged adapter

## Objectives
- Capture HTTP and HTTPS traffic
- Analyze request/response headers
- Understand data exposure over HTTP vs HTTPS

## Traffic Captured

### HTTP Request Sample
```bash
curl http://httpbin.org/get
```

### HTTPS Request Sample
```bash
curl https://httpbin.org/get
```

### Filters and Analysis in Wireshark
http only
```
http
```
https (tls)
```
tls
```
ip/host
```
ip.addr == 192.168.xx.xx
```
