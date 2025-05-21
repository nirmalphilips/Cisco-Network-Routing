## Requirements

### Overview
- **Client:** NoPlanetB, an environmental-sustainability consultancy producing white papers for governments and industry.  
- **Scope:** Migrate existing network infrastructure (Head Office, Research Centre, three Research Sites, Monitoring Station) to a new location using Cisco Packet Tracer

### Topology & Addressing
- **Routers to configure:**  
  - **NoPlanetBHO (Head Office)**  
    - Convert its IPv6 WAN IP (`7b6c:f189:ab2f:1ab4:3e1a:0ad4:5472:2f2a`) to IPv4.  
    - Define IPv4 link to the Monitoring Station (address/netmask of your choice with justification).  
  - **NoPlanetBRC (Research Centre)**  
    - Convert its IPv6 WAN IP (`04be:5cde:0e76:eef7:04be:7cde:d101:5f46`) to IPv4.  
    - Define IPv4 link to the Monitoring Station with justification.  
  - **Monitoring Station Router**  
    - Assign an internal IPv4 subnet (justify network & mask).  
    - Allocate IPv4 addresses for each attached device.  
  - **Research Sites Home Router**  
    - Define IPv4 link(s) to the Monitoring Station (justify network & mask).  
    - Create three IPv4 LAN subnets—one per micro-site.

### Routing Requirements
- **Internal (RC & Sites):** Static routing, RIP, or a mix—your choice for site-to-site reachability.  
- **Internet (HO ↔ RC via BGP):** Choose one scenario:  
  1. **Green** (2 BGP routes)  
  2. **Orange** (4 BGP routes)  
  3. **Red** (3 BGP routes + RIP-mesh iBGP simulate)

### Security & Legality
- Implement console/vty authentication on **every** router.  
- Configure appropriate `motd`, `login` and `exec` banners to comply with company policy


