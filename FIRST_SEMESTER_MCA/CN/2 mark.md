Here are concise answers tailored to your **Part-I** questions:

---

### **Part-I (2 x 10 = 20 Marks)**

**a) Define the term 'protocol' in the context of computer networks.**  
A **protocol** is a set of rules and conventions that govern the communication between devices on a network. It ensures reliable data exchange by defining how data is formatted, transmitted, and received. Examples include HTTP, TCP, and FTP.  

---

**b) Describe the key difference between analog and digital signals.**  
**Analog signals** are continuous waveforms that represent data such as sound, light, or temperature. For example, voice on a telephone is an analog signal.  

**Digital signals** are discrete and use binary (0s and 1s) to represent data. They are commonly used in computers and devices, such as in emails or digital audio recordings.
- **Analog signals** are continuous waveforms representing data, such as sound or light.  
- **Digital signals** are discrete, using binary (0s and 1s) to represent data.  
**Example:** Voice on a telephone (analog), emails (digital).

---

**c) What is the OSI model, and how does it differ from the TCP/IP model?**  
The **OSI model** is a 7-layer framework (Physical, Data Link, Network, Transport, etc.) for understanding network functions.  
The **TCP/IP model** has 4 layers (Application, Transport, Internet, Network Access) and focuses on practical implementation.  
**Difference:** OSI is theoretical; TCP/IP is widely used in real-world networking.

---

**d) Explain the concept of 'Layering' in computer networks.**  
**Layering** divides the communication process into separate levels, where each layer handles a specific aspect (e.g., data transfer, addressing).  
- It simplifies network design and troubleshooting.  
- Examples: OSI and TCP/IP models.

---

**e) List two common transmission impairments in data communication.**  
1. **Attenuation:** Loss of signal strength over distance.  
2. **Noise:** Unwanted signals interfering with the original data (e.g., electromagnetic interference).  

---

**f) What are CRC codes, and what is their purpose in data communication?**  
**Cyclic Redundancy Check (CRC)** is an error-detection method. It generates a checksum value from data and appends it to the message. The receiver recalculates the checksum to verify data integrity.  

---

**g) Define the term 'multiplexing' in network communication.**  
**Multiplexing** is a technique to combine multiple signals for simultaneous transmission over a single communication channel.  
Types include **TDM (Time Division Multiplexing)** and **FDM (Frequency Division Multiplexing).**

---

**h) Describe the purpose of a 'hub' in networking.**  
A **hub** is a simple networking device that connects multiple devices in a LAN. It broadcasts incoming data to all connected devices, leading to higher collisions.

---

**i) What is meant by 'store and forward packet switching'?**  
In **store-and-forward packet switching**, a node receives the entire packet, stores it temporarily, checks for errors, and then forwards it to the next node.  
It ensures error-free data transmission.

---

**j) Explain the term 'sliding window protocol' and its use in networking.**  
The **sliding window protocol** is a flow control mechanism used in reliable data transfer.  
- The sender can send multiple frames before needing an acknowledgment (ACK).  
- It improves efficiency by using a window size for managing unacknowledged frames.  

--- 

### Part-I: 2-Mark Questions

(a) **Differentiate between IPv4 and IPv6.**  
**Module IV: Internetworking**  
- IPv4 uses 32-bit addresses, allowing approximately 4.3 billion unique addresses.  
- IPv6 uses 128-bit addresses, providing a vastly larger address space.  
- IPv4 uses dot-decimal notation (e.g., 192.168.0.1), while IPv6 uses hexadecimal separated by colons (e.g., 2001:0db8::1).  

---

(b) **What is a frame?**  
**Module I: Overview of the Internet**  
A frame is a data packet at the Data Link Layer, encapsulating data for transmission over a physical medium. It includes headers and trailers for synchronization, addressing, and error detection.  

---

(c) **Differentiate between LAN and MAN.**  
**Module I: Overview of the Internet**  
- LAN (Local Area Network): Covers a small area like a home or office, typically using Ethernet.  
- MAN (Metropolitan Area Network): Covers a larger area like a city, often using technologies like fiber optics or cable.  

---

(d) **What is the use of a router?**  
**Module III: Connecting Devices**  
A router directs data packets between different networks. It determines the best path for data to travel and connects devices to the internet.  

---

(e) **What is WLAN?**  
**Module II: Data Link Layer**  
WLAN (Wireless Local Area Network) is a wireless network that allows devices to connect and communicate using Wi-Fi, eliminating the need for cables.  

---

(f) **Explain the usage of Ethernet.**  
**Module II: Data Link Layer**  
Ethernet is a wired communication standard used for LANs, offering high-speed data transfer and reliable connectivity using cables like CAT5 or CAT6.  

---

(g) **Define the data rate limit.**  
**Module I: Overview of the Internet**  
The data rate limit refers to the maximum amount of data transmitted over a communication channel per second, often determined by the medium's bandwidth and signal quality.  

---

(h) **Explain differences between UDP and TCP.**  
**Module V: Transport Protocols**  
- TCP (Transmission Control Protocol) is connection-oriented, ensuring reliable data delivery.  
- UDP (User Datagram Protocol) is connectionless, faster, but does not guarantee delivery or order.  

---

(i) **Why do we use HTTP?**  
**Module V: Application Layer**  
HTTP (HyperText Transfer Protocol) is used to transfer web pages and other resources over the internet, enabling communication between clients (browsers) and servers.  

---

(j) **Explain the concept of a periodic analog signal.**  
**Module I: Overview of the Internet**  
A periodic analog signal repeats a pattern over time, such as a sine wave. Examples include radio waves or alternating current (AC) signals.

### Part-I: 2-Mark Questions

(a) **What is meant by data communication?**  
**Module I: Overview of the Internet**  
Data communication refers to the exchange of data between devices or systems over a communication medium, such as cables or wireless networks. It involves sending and receiving data in the form of signals, ensuring the accurate and timely transfer of information.

---

(b) **What are the responsibilities of the data link layer?**  
**Module II: Data Link Layer**  
The data link layer ensures reliable communication between two directly connected devices. It handles framing, error detection and correction, flow control, and media access management to prevent data collision and ensure smooth data transmission.

---

(c) **What is ARQ?**  
**Module II: Data Link Layer**  
ARQ (Automatic Repeat Request) is an error-control mechanism in data communication. It ensures data reliability by retransmitting corrupted or lost data packets based on feedback from the receiver.

---

(d) **Write short notes on Ethernet.**  
**Module II: Data Link Layer**  
Ethernet is a widely used LAN technology that defines a set of protocols for transmitting data over wired networks using frames. It uses CSMA/CD (Carrier Sense Multiple Access with Collision Detection) to manage access to the shared medium and supports speeds ranging from 10 Mbps to 100 Gbps.

---

(e) **What is a Hub?**  
**Module III: Connecting Devices**  
A hub is a basic networking device that connects multiple devices in a LAN, allowing data to be transmitted between them. It works by broadcasting data to all connected devices, without distinguishing between them, which can lead to collisions.

---

(f) **Define LAN.**  
**Module I: Overview of the Internet**  
A LAN (Local Area Network) is a network that connects devices within a limited geographical area, such as a home, office, or building. It typically uses Ethernet or Wi-Fi technology to facilitate high-speed data transfer.

---

(g) **Differentiate between IPv4 and IPv6.**  
**Module IV: Internetworking**  
- IPv4 uses 32-bit addresses, allowing for approximately 4.3 billion unique IP addresses.  
- IPv6 uses 128-bit addresses, allowing for an extremely large address space to accommodate the growing number of devices.  
- IPv6 also supports better security and routing features compared to IPv4.

---

(h) **What is the purpose of the Domain Name System?**  
**Module V: Application Layer**  
The Domain Name System (DNS) is used to translate human-readable domain names (like www.example.com) into IP addresses (like 192.168.1.1), enabling browsers and other applications to locate and communicate with servers over the internet.

---

(i) **What is TELNET?**  
**Module V: Application Layer**  
TELNET is a protocol used to remotely access and manage devices over a network. It provides a command-line interface for users to log into remote systems, but it lacks encryption, making it less secure compared to modern alternatives like SSH.

---

(j) **What is FTP?**  
**Module V: Application Layer**  
FTP (File Transfer Protocol) is used to transfer files between a client and a server over a network. It supports both uploading and downloading of files and provides commands to manage directories and file permissions.
