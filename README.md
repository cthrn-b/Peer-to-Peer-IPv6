# Peer-to-Peer IPv6 Network using Packet Tracer

## Objective
To configure a peer-to-peer IPv6 network using Cisco Packet Tracer with five computers connected through a switch.

## Network Setup
1. **Devices:**
   - 5 PCs
   - 1 Switch (e.g., Cisco 2960)
   - Copper straight-through cables

2. **IPv6 Address Allocation (Global Unicast - 2001:db8:acad::/64):**
   - PC1: `2001:db8:acad::1/64`
   - PC2: `2001:db8:acad::2/64`
   - PC3: `2001:db8:acad::3/64`
   - PC4: `2001:db8:acad::4/64`
   - PC5: `2001:db8:acad::5/64`

## Configuration Steps
1. **Set Up Devices**
   - Place PCs and Switch in Packet Tracer.
   - Connect PCs to the switch using copper straight-through cables.

2. **Assign IPv6 Addresses**
   - Navigate to each PC’s desktop → IP Configuration.
   - Enable IPv6 and assign the provided IPv6 addresses.

3. **Test Connectivity**
   - Use the `ping` command in the command prompt to verify connectivity between all PCs.
   - Example: `ping 2001:db8:acad::2` from PC1.

4. **Link-Local Address Testing 
   - Check assigned link-local addresses (`fe80::/10` range).
   - Ping other PCs using their link-local addresses.

5. **Enable Additional Services
   - Set up PC1 as a web server (enable HTTP service in Packet Tracer).
   - Access the webpage from other PCs using `http://2001:db8:acad::1`.
