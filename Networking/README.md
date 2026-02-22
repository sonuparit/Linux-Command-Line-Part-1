# 🚀 Linux Networking for DevOps Engineers

> A practical, production-focused reference guide for modern Linux
> networking, debugging, and infrastructure troubleshooting.

This repository contains regularly used and **latest networking
commands** used by DevOps engineers in real-world production
environments.

---

# 🌐 Core Networking Commands

## 🔎 1. ip (Modern Replacement for ifconfig, route, arp)

### Show IP Addresses

```bash
ip addr
```

### Show Routing Table

```bash
ip route
```

### Show ARP / Neighbor Table

```bash
ip neigh
```

### Bring Interface Up/Down

```bash
sudo ip link set eth0 up
sudo ip link set eth0 down
```

---

## 🌍 2. ping -- Connectivity Test

```bash
ping google.com
```

Used to verify: - Network reachability - Packet loss - Latency

---

## 🛰 3. traceroute / tracepath -- Path Analysis

```bash
traceroute google.com
tracepath google.com
```

Used to identify: - Routing path - Network bottlenecks - ISP-level
issues

---

## 🌐 4. dig -- DNS Debugging (Modern Alternative to nslookup)

```bash
dig google.com
dig google.com @8.8.8.8
dig example.com MX
```

Used for: - DNS resolution troubleshooting - Checking propagation -
Inspecting TTL values

---

## 🔥 5. ss -- Modern Socket Statistics (Replacement for netstat)

```bash
ss -tulnp
```

Used to: - Check listening ports - Identify processes using ports -
Debug service conflicts

---

## 🛠 6. nc (Netcat) -- Port Testing

```bash
nc -zv server.com 443
```

Used for: - Testing TCP connectivity - Debugging firewall rules -
Checking internal service communication

---

## 🌍 7. wget & curl -- HTTP Testing & Downloads

### Download File

```bash
wget https://example.com/file.zip
```

### Test API / HTTP Endpoint

```bash
curl -I https://example.com
```

Used for: - Health checks - CI/CD validation - Deployment verification

---

## 🧱 8. nftables -- Modern Linux Firewall

### View Rules

```bash
sudo nft list ruleset
```

### Check Service Status

```bash
sudo systemctl status nftables
```

Used for: - Firewall configuration - Traffic filtering - Production
hardening

---

## 📡 9. watch -- Real-Time Monitoring

```bash
watch -n 2 ss -tuln
```

Used to monitor: - Port changes - Kubernetes pods - Disk and network
stats

---

# 🧠 Production Debugging Workflow

When troubleshooting a service outage:

1.  Check DNS → `dig domain.com`
2.  Check connectivity → `ping server-ip`
3.  Check route → `ip route`
4.  Check port listening → `ss -tulnp`
5.  Test connection → `nc -zv server 443`
6.  Verify firewall → `nft list ruleset`

---

# 🐳 Container & Kubernetes Relevance

These commands are essential for:

- Debugging Docker container networking
- Troubleshooting Kubernetes Services
- Verifying NodePort and Ingress exposure
- Diagnosing overlay network issues

---

# 🎯 Why This Matters for DevOps

Strong networking fundamentals allow engineers to:

- Diagnose production outages faster
- Understand cloud networking behavior
- Debug CI/CD deployment issues
- Work confidently with Kubernetes and microservices
- Secure Linux servers properly

---

# 📌 Skills Demonstrated

- Linux Networking Fundamentals
- Production Debugging Approach
- Firewall & Security Awareness
- DNS and Routing Analysis
- Modern Linux Tooling (iproute2, nftables)

---

# 🏆 Ideal For

- DevOps Engineers
- Cloud Engineers
- SRE Professionals
- Linux System Administrators

---

# 📚 Continuous Improvement

This repository will continue evolving with:

- Advanced packet inspection (tcpdump, Wireshark)
- Deep Kubernetes networking concepts
- Load balancer debugging
- Cloud networking case studies

---

> Networking is not optional in DevOps. It is foundational.
