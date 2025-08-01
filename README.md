# 🎯Subnet -
A Subnet Calculator takes an IP address and subnet mask (or CIDR) and calculates:

1. Network address
2. Broadcast address
3. First/last usable IP
4. Number of hosts
5. Wildcard mask
6. IP class
7. CIDR notation

# 🏷Calculation Table

| Item            | How to Find (Simple)                         | Example (192.168.1.10/24)      |
|-----------------|-----------------------------------------------|---------------------------------|
| **Network**     | All host bits = 0                            | **192.168.1.0**                 |
| **Broadcast**   | All host bits = 1                            | **192.168.1.255**               |
| **1st Usable**  | Network + 1                                  | **192.168.1.1**                  |
| **Last Usable** | Broadcast - 1                                | **192.168.1.254**                |
| **Hosts**       | 2^(host bits) - 2                            | **254**                          |
| **Wildcard**    | 255 - subnet mask                            | **0.0.0.255**                    |
| **Class**       | Check 1st number: 192 = Class C               | **C**                            |
| **CIDR**        | Count 1’s in mask (255.255.255.0 = /24)      | **/24**                          |
