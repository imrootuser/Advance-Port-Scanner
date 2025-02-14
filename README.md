# Advanced Port Scanner

## Overview
The **Advanced Port Scanner** is a Python-based cybersecurity tool that allows users to scan a target IP or hostname for open ports efficiently. This tool helps security professionals and ethical hackers analyze network security and detect vulnerabilities.

## Features
- Fast multi-threaded scanning
- Scans a range of ports or specific ports
- Identifies open and closed ports
- Supports both TCP and UDP scanning
- Custom timeout for better accuracy

## Installation
### Prerequisites
Ensure you have Python installed (version 3.x recommended). You can download it from [Python.org](https://www.python.org/downloads/).

### Clone the Repository
```bash
git clone https://github.com/imrootuser/Advanced-Port-Scanner.git
cd advanced-port-scanner
```

### Install Required Dependencies
```bash
pip install -r requirements.txt
```

## Usage
### Basic Port Scan
```bash
python scanner.py -t <TARGET_IP> -p 1-65535
```
Example:
```bash
python scanner.py -t 192.168.1.1 -p 20,21,22,80,443
```

### Scan with Custom Timeout
```bash
python scanner.py -t <TARGET_IP> -p 1-1000 --timeout 1
```

### UDP Scan Mode
```bash
python scanner.py -t <TARGET_IP> -p 53,123 --udp
```

## Example Output
```
Scanning 192.168.1.1...
Port 22 (SSH) is open
Port 80 (HTTP) is open
Port 443 (HTTPS) is open
Scan completed in 5.32 seconds
```

## Contribution
Feel free to contribute by opening an issue or creating a pull request!

## Disclaimer
This tool is for **educational and authorized security testing purposes only**. Unauthorized scanning of networks is illegal. Use responsibly.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
**Author:** imrootuser  
**GitHub:** [imrootuser](https://github.com/imrootuser)
