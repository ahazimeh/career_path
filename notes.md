## Learning Techniques

### Brain Modes
- **Focused Mode**: Concentrated attention
- **Diffused Mode**: Relaxed thinking (valuable for problem-solving)

### Memory Principles
- Short-term memory capacity: ~4 items
- Long-term memory formation requires spaced repetition
- Hydration is crucial (73% of brain is water)

### Memorization Techniques
1. **Make it interesting**: Use humor or exaggeration
2. **Visual imagery**: Create mental pictures
3. **Memory pegs**: Associate numbers with objects
   ```
   1 = bun
   2 = shoe
   3 = tree
   4 = door
   5 = hive
   6 = sticks
   7 = heaven
   8 = gate
   9 = wine
   10 = hen
   ```
4. **Set to music**: Use melodies
5. **Acronyms**: First letter of each item
6. **Retrieval practice**: Recall before learning
7. **Flashcards**: Two-sided information cards
8. **Memory palace**: Place items in familiar locations

### Overcoming Procrastination
1. Self-talk: Give yourself clear instructions
2. Focus on time blocks, not tasks (25-minute sessions)
3. Start with easier tasks to build momentum
4. Eliminate distractions
5. Reward yourself after completing work sessions

### Chunking
- Group related information together
- Create stories to connect chunks

### Top 10 Learning Tips
1. Exercise before studying to reduce stress
2. Avoid comparing yourself to others
3. Study in groups
4. Start with easy questions in exams
5. Use highlighters sparingly
6. Test your understanding by solving problems independently
7. Study in different environments
8. Manage anxiety (reframe as excitement)
9. For multiple choice: hide options and answer first
10. Take breaks before reviewing answers

### Skill Acquisition
- 20 hours to learn a new skill:
  1. Break skills into smaller components
  2. Learn enough to self-correct
  3. Remove practice barriers
  4. Practice at least 20 hours

# Networking and Learning Techniques - Knowledge Library

## Network Fundamentals

### Basic Components
- **Interface**: Converts data to electrical signals (transmitter) and electrical signals to data (receiver)
- **Fiber**: Converts bits to light signals
- **Network Protocol**: Standard set of rules for communication

### Network Topologies

#### 1. Bus Topology
- Single central cable with all devices connected to it
- **Advantages**: Simple implementation
- **Disadvantages**:
  - Low performance (entire network busy with each transmission)
  - Single point of failure
  - Data sent to all devices

#### 2. Ring Topology
- Devices connected in a circular arrangement
- **Advantages**:
  - Easy implementation
  - No data collision
- **Disadvantages**:
  - Data must pass through intermediate devices
  - Single point of failure
  - Difficult to add new devices

#### 3. Mesh Topology
- Each device connected to all other devices
- **Advantages**:
  - Point-to-point links
  - Better security
- **Disadvantages**:
  - More expensive
  - Complex network management

#### 4. Star Topology
- Central device with all other devices connected to it
- **Advantages**:
  - Inexpensive
  - Scalable
- **Disadvantages**:
  - Single point of failure (can be mitigated with redundant switches)

### Data Transmission Types

#### Casting Methods
1. **Unicast**: One-to-one communication
2. **Multicast**: One-to-many communication (specific group)
3. **Broadcast**: One-to-all communication
   - Limited broadcast: All devices in same network
   - Direct broadcast: All devices in another group

#### Transmission Modes
1. **Simplex**: One-way communication (e.g., radio)
2. **Half-Duplex**: Two-way communication, one direction at a time
3. **Full-Duplex**: Simultaneous two-way communication (e.g., phone calls)

## Network Types

### Geographic Classification
1. **PAN** (Personal Area Network): 10-15m range (e.g., mobile to laptop)
2. **LAN** (Local Area Network): Limited geographic area
3. **WLAN** (Wireless Local Area Network): Wireless implementation of LAN
4. **CAN** (Campus Area Network): Two or more LANs
5. **MAN** (Metropolitan Area Network): City-wide coverage
6. **SAN** (Storage Area Network): Specialized for storage devices
7. **WAN** (Wide Area Network): Large geographic coverage

### Host Role Classification
- **Peer-to-Peer (P2P)**: Equal roles for all devices
- **Client/Server**: Dedicated servers providing services to clients

## OSI Model Layers

1. **Application Layer**: User interfaces and protocols
2. **Presentation Layer**: Data translation, compression, encryption
3. **Session Layer**: Session management, transmission mode control
4. **Transport Layer**:
   - Segmentation (ports and sequence numbers)
   - Flow control
5. **Network Layer**: Logical addressing and routing
6. **Data Link Layer**:
   - Physical addressing (MAC addresses)
   - Media access
   - Error detection and correction:
     - Parity checking
     - Checksum
     - CRC
   - Uses CSMA protocol to monitor traffic
7. **Physical Layer**: Converts bits to signals for transmission

## Networking Services

### DNS (Domain Name System)
- Components:
  - DNS Resolver: Initial point of contact for requests
  - Root Name Server: Four servers for all websites
  - TLD Server: Domain-specific servers (e.g., .com)
  - Authoritative Name Server: Verifies user access authorization

### DHCP (Dynamic Host Configuration Protocol)
- Process:
  1. DHCP Discover: Broadcast request (0.0.0.0 → 255.255.255.255)
  2. DHCP Offer: Server proposes IP, subnet, lease time
  3. DHCP Request: Client accepts IP address
  4. DHCP Acknowledgment: Server confirms configuration
- Features:
  - Address reservation for specific devices
  - Lease-based allocation

### ARP (Address Resolution Protocol)
- Maps IP addresses to MAC addresses
- Maintains ARP cache of recently communicated devices

## Network Devices

### Hub
- **Function**: Connects devices in a single network
- **Characteristics**:
  - Physical layer device
  - Broadcasts data to all connected devices
  - Half-duplex operation
  - Poor bandwidth utilization
  - Limited security

### Switch
- **Function**: Intelligent connection of devices
- **Characteristics**:
  - Layer 2 device (Data Link)
  - Uses MAC addresses for targeted transmission
  - Full-duplex operation
  - Multiple collision domains
  - Efficient bandwidth usage
  - Enhanced security

### Router
- **Function**: Connects different networks
- **Characteristics**:
  - Layer 3 device (Network)
  - Uses routing tables
  - Makes path decisions

## Network Security

### Firewall Types
1. **Packet Filtering Firewall**: Examines packet headers only
2. **Stateful Inspection Firewall**: Tracks connection states
3. **Proxy Firewall**: Adds intermediary layer
4. **Application Firewall**: Protects web applications (WAF)
5. **Next Generation Firewall**:
   - URL and web filtering
   - Deep Packet Inspection (DPI)
   - Intrusion Prevention System (IPS)

### DMZ (Demilitarized Zone)
- Separates:
  - Trusted network (internal)
  - Untrusted network (internet)
- Types:
  - Single firewall DMZ
  - Dual firewall DMZ
- Uses:
  - Public access to specific services (e.g., mail server)
  - Home router DMZ hosts (used by gamers)

## Network Configuration

### Port Numbers
- Range: 0-65535
- Categories:
  - System/Well-known ports: 0-1023
  - User/Registered ports: 1024-49151
  - Dynamic/Private ports: 49152-65535
- Check connections with `netstat -n`

### VLAN (Virtual Local Area Network)
- Divides single physical network into multiple logical networks
- VLAN ID range: 0-4096 (first and last not used)
- Port types:
  - Access port: Connects devices to switch
  - Trunk port: Connects switches, carries traffic between VLANs
- Uses 802.1Q (Dot1q) tagging

### VPN (Virtual Private Network)
- Types:
  - Split tunnel: Only company traffic through VPN
  - Full tunnel: All traffic through VPN

### IP Addressing
- Classes: A (large organizations), B, C (home use)
- NAT (Network Address Translation): Maps private to public addresses
  - Static NAT: Manual mapping
  - Dynamic NAT: Automatic mapping
  - PAT (Port Address Translation): Many-to-one mapping using ports

### Wireless Networking
- Frequency bands:
  - 2.4 GHz: Better range and wall penetration, more crowded (11 channels, 3 non-interfering)
  - 5 GHz: Less interference, shorter range (25 non-interfering channels)
- Identifiers:
  - BSSID (Basic Service Set Identifier): Unique numerical ID
  - SSID (Service Set Identifier): Wi-Fi network name

### Cloud Computing
- Deployment models:
  - Public cloud
  - Private cloud
  - Hybrid cloud (public for backup)
- Service models:
  - IaaS (Infrastructure as a Service): Hardware only
  - PaaS (Platform as a Service): Deployment platform
  - SaaS (Software as a Service): Complete application hosting

Operating System Command Line Tools

CMD: Command line interface (default OS command shell in Windows)
PowerShell: Enhanced command shell with more features than CMD
Windows Security Features:

Ransomware protection
Windows Security Center
