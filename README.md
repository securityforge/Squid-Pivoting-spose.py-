# Squid-Pivoting-spose.py-
Used to pivot through an exposed Squid proxy (port 3128) to access internal network services not directly reachable from attacker machine.

## 🎯 Purpose

* Exploit misconfigured **open Squid proxy (3128)**
* Perform internal port scanning through proxy tunnel
* Enumerate hidden/internal services not exposed externally
* Identify attack surface inside segmented network
* Enable pivoting for lateral movement
* Transition from external foothold → internal access chain

```
python3 spose.py --proxy http://<<target-ip-addr>>:3128 --target <<target-ip-addr>>
```
output looks like
```
Scanning default common ports
Using proxy address http://<<target-ip-addr>>:3128
<<target-ip-addr>>:3306 seems OPEN
<<target-ip-addr>>:8080 seems OPEN
```
