# checkproxy
A tool for testing proxy server availability.

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![Requests](https://img.shields.io/badge/Requests-2.25+-green.svg)
![PySocks](https://img.shields.io/badge/PySocks-1.7+-orange.svg)

## About the Project
checkproxy is an automated tool for testing proxy server availability, demonstrating principles of network interaction, proxy type detection, and response time measurement.

### Features
- Automatic detection of proxy types (HTTP, HTTPS, SOCKS4, SOCKS5)
- Availability testing via httpbin.org
- Response time measurement in milliseconds
- Support for proxy.txt format (one proxy per line)
- Saves working proxies to working_proxy.txt
- Automatic duplicate filtering
- Statistics on working proxy types
- Display of date and time of testing
- Simple and clear code structure

### Input Format
Create a `proxy.txt` file in the program folder, one proxy per line:
```
192.168.1.1:8080
proxy.example.com:3128
socks5://127.0.0.1:1080
```

### Output Format
Working proxies are saved to `working_proxy.txt`:
```
http://192.168.1.1:8080 # 125ms
socks5://127.0.0.1:1080 # 89ms
```
