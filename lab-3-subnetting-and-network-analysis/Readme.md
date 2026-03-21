## Step-by-Step Subnet Calculation

### Given:
IP Address: 192.168.1.10  
Subnet Mask: 255.255.255.0 (/24)

---

### Step 1: Identify Subnet Mask

255.255.255.0 means:

- First 3 octets = network portion  
- Last octet = host portion  

---

### Step 2: Calculate Total Number of IP Addresses

Formula:

Total IPs = 2^(number of host bits)

Here:
- /24 → 24 bits network  
- Remaining = 32 - 24 = 8 host bits  

So:

Total IPs = 2^8 = 256  

---

### Step 3: Find Network Address

Rule:
Set all host bits to 0  

So:

192.168.1.10 → 192.168.1.0  

Network Address = 192.168.1.0  

---

### Step 4: Find Broadcast Address

Rule:
Set all host bits to 1  

So:

192.168.1.255  

Broadcast Address = 192.168.1.255  

---

### Step 5: Find Usable Host Range

- First usable IP = Network + 1  
- Last usable IP = Broadcast - 1  

So:

192.168.1.1 → 192.168.1.254  

---

### Step 6: Calculate Usable Hosts

Formula:

Usable hosts = Total IPs - 2  

(1 network + 1 broadcast)

So:

256 - 2 = 254 hosts  

---

## Final Answer Summary

- Network Address: 192.168.1.0  
- Broadcast Address: 192.168.1.255  
- Usable Range: 192.168.1.1 – 192.168.1.254  
- Total Hosts: 254  