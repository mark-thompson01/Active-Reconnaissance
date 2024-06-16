# Active-Reconnaissance Lab

This lab outlines performing host discovery, port scanning, service version detection, and vulnerability scanning and detection using Nmap. The lab was conducted in a controlled environment to demonstrate various reconnaissance techniques.

## Table of Contents

- [Introduction](#introduction)
- [Host Discovery](#host-discovery)
  - [Nmap Host Discovery](#nmap-host-discovery)
  - [ARP Scan](#arp-scan)
  - [FPing](#fping)
  - [Passive Reconnaissance with Wireshark](#passive-reconnaissance-with-wireshark)
  - [Screenshots](#screenshots-host-discovery)
- [Port Scanning and Host Fingerprinting](#port-scanning-and-host-fingerprinting)
  - [Nmap Port Scanning](#nmap-port-scanning)
  - [Nmap Service Version Detection](#nmap-service-version-detection)
  - [Fingerprinting with Nmap Scripts](#fingerprinting-with-nmap-scripts)
  - [Screenshots](#screenshots-port-scanning)
- [Web Server Enumeration on Port 80](#web-server-enumeration-on-port-80)
  - [Screenshots](#screenshots-web-server-enumeration)
- [Conclusion](#conclusion)
- [Contact](#contact)

## Introduction

This document contains step-by-step guides for performing active reconnaissance using Nmap and other tools. It covers host discovery, port scanning, service version detection, and web server enumeration.

## Host Discovery

### Nmap Host Discovery

```bash
# Perform a ping scan to discover live hosts on the network
nmap –sn 10.38.1.1/24


### ARP Scan

# Perform an ARP scan to discover hosts on the local network
arp-scan –localnet

### FPing

# Use fping to discover live hosts
fping -a -g 10.38.1.1/24

## Passive Reconnaissance with Wireshark

Use Wireshark to perform passive reconnaissance on the active network by capturing and analyzing network traffic.


## Screenshots Host Discovery

### Nmap Host Discovery

### ARP Scan



### Fping

### Wireshark


## Port Scanning and Host Fingerprinting

### Nmap Port Scanning

# Perform a SYN scan and service version detection
nmap –sS –sV –reason 10.38.1.114

# Perform a full port scan and service version detection
nmap –sS –sV –p- --reason 10.38.1.114

# Perform a SYN scan, service version detection, and UDP scan
nmap –sS –sV –sU –reason 10.38.1.114

# Perform a port scan for ports 1-10000 and service version detection
nmap –sS –sV –p1-10000 –reason 10.38.1.114


## Nmap Service Version Detection

After identifying open ports, perform service version detection on individual ports to gather more information.

### Fingerprinting with Nmap Scripts

Use Nmap scripts to fingerprint services and gather detailed information.

## Screenshots Port Scanning

### SYN Scan and Service Detection

### Full Port Scan

### SYN and UDP Scan

### Port Scan (1-10000)


## Web Server Enumeration on Port 80

Enumerate the web server running on port 80 to gather information about the web application and its components.

## Screensshots Web Server Enumeration

### Web Server Enumeration


Conclusion

This lab demonstrates various techniques for active reconnaissance, including host discovery, port scanning, service detection, and web server enumeration. These skills are essential for both red team and blue team activities in cybersecurity.










