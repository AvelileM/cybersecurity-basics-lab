# Basic Network Investigation

## Purpose

The purpose of this exercise is to investigate basic network information and understand how a computer communicates with other systems.

## Environment

This investigation was performed using Git Bash on Windows.

## 1. Hostname

### Command

```bash
hostname
```

### Result

The command returned my computer's hostname.

### What I Learned

The hostname is used to identify a computer on a network.

## 2. Network Configuration

### Command

```bash
ipconfig
```

### What I Investigated

I used `ipconfig` to examine the network configuration of my Windows computer.

I looked for:

* IPv4 address
* Subnet mask
* Default gateway

### What I Learned

An IP address identifies a device/interface on a network.

A default gateway provides a route for traffic leaving the local network.

> Note: I did not publish my actual IP address in this repository.

## 3. Connectivity Test

### Command

```bash
ping google.com
```

### What I Observed

The command sent network requests and displayed responses from the destination.

### What I Learned

`ping` can be used to test whether a destination is reachable and to measure the approximate round-trip time for the request.

## 4. DNS Investigation

### Command

```bash
nslookup google.com
```

### What I Observed

The command returned DNS information associated with `google.com`.

### What I Learned

DNS translates human-readable domain names into IP addresses that computers can use to communicate with network destinations.

## Security Relevance

Understanding networking is important in cybersecurity because systems communicate across networks.

Basic network information can help security professionals investigate connectivity problems, identify systems and understand how network traffic moves between devices.

## Key Observation

This investigation showed me that several different components are involved when a computer communicates with a website, including IP addressing, routing and DNS.

## Next Step

The next exercise will investigate basic security checks on the system.
