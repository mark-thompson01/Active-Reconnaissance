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


## Introduction

This document contains step-by-step guides for performing active reconnaissance using Nmap and other tools. It covers host discovery, port scanning, service version detection, and web server enumeration. All activity was performed in a virtualized contained environment with three VMs. In this example, arp-scan, nmap, and fping are all utilized to perform network host discovery while the host fingerprinting stage primarily focusing on a Metasploitable2 VM.

## Host Discovery

### ARP, Fping, and Nmap Ping Scan:

Perform an arp scan, nmap ping scan, and an pfing scan to discover what hosts are connected to the local network. 

![arp-scan-nmap-sn](images/arp-scan-nmap-sn.png)

![fping](images/fping.png)


### Passive Reconnaissance with Wireshark

Use Wireshark to perform passive reconnaissance on the active network by capturing and analyzing network traffic. 


## Port Scanning and Host Fingerprinting

Perform a SYN scan and service version detection. 

![Port Scanning and Service Detection](images/Port%20Scanning%20and%20Service%20Detection.png)



Perform a full port scan and service version detction

![Full Port Scan](images/Full%20Port%20Scan.png)


Perform a SYN scan, service version detection, and UDP scan: 

![SYN-sV-sU](images/SYN-sV-sU.png)

Perform a port scan for ports 1-10000 and service version detection: 

![p1-10000](images/p1-10000.png)



## Fingerprinting with Nmap Scripts

Use Nmap scripts to fingerprint services and gather detailed information. 

![nmapftpanon](images/nmapftpanon.png)

![nmapftp-syst](images/nmapftp-syst.png)

![nmapftpvuln](images/nmapftpvuln.png)


![nmapssh-auth-methods](images/nmapssh-auth-methods.png)

![nmapssh-hostkey](images/nmapssh-hostkey.png)

![nmapssh2-enum-algos](images/nmapssh2-enum-algos.png)


![nmapsmb-os-discovery](images/nmapsmb-os-discovery.png)

![nmapsmb-security-mode](nmapsmb-security-mode.png)



## Web Server Enumeration on Port 80

Enumerate the web server on port 80 to gather information about the web application and its components. 













