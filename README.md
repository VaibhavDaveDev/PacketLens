# PacketLens: Network Traffic Analyzer

<div align="center">
  <p><strong>A powerful, Java-based packet capture and network traffic analysis tool</strong></p>
  <p>
    <a href="#features">Features</a> •
    <a href="#installation">Installation</a> •
    <a href="#usage">Usage</a> •
    <a href="#supported-protocols">Supported Protocols</a> •
    <a href="#architecture">Architecture</a> •
    <a href="#requirements">Requirements</a> •
    <a href="#contributing">Contributing</a> 
  </p>
</div>

## Overview

PacketLens is a robust network packet analyzer that provides real-time monitoring and analysis of network traffic. Built with Java and the Jpcap library, it allows system administrators, network engineers, and security professionals to capture, visualize, and analyze network packets for troubleshooting, security monitoring, and performance optimization.

Whether you're debugging network issues, monitoring for suspicious activities, or analyzing network performance, PacketLens provides a comprehensive toolkit for deep packet inspection and protocol analysis.

## Features

- **🔍 Real-time Packet Capture**: Monitor live network traffic from any network interface
- **📊 Protocol Analysis**: Deep packet inspection across multiple protocol layers
- **📈 Traffic Statistics**: Generate comprehensive statistics on network usage patterns
- **🔄 Multi-protocol Support**: Analyze packets for numerous protocols across all network layers
- **📁 File Operations**: Save and load packet captures for later analysis
- **📊 Data Visualization**: Visual representation of traffic patterns and protocol distribution
- **🔧 Customizable Interface**: Configurable display options and filters
- **🔒 Advanced Filtering**: Filter traffic based on various parameters (protocol, port, IP, etc.)
- **📱 Cross-platform**: Works on Windows, Linux, and macOS systems

## Installation

### Prerequisites

- Java Runtime Environment (JRE) 8 or higher
- Jpcap library (included in the release)
- WinPcap (Windows) or libpcap (Linux/macOS)

### Setup Instructions

1. **Install WinPcap/libpcap**
   - Windows: Download and install [WinPcap](https://www.winpcap.org/install/)
   - Linux: `sudo apt-get install libpcap-dev`
   - macOS: `brew install libpcap`

2. **Download PacketLens**
   ```
   git clone https://github.com/VaibhavDaveDev/PacketLens.git
   ```

3. **Compile the application**
   ```
   cd PacketLens
   javac -d bin src/**/*.java
   ```

4. **Run PacketLens**
   ```
   java -cp bin;lib/* app.NetPackSniff
   ```
   (On Linux/macOS, use `:` instead of `;`: `java -cp bin:lib/* app.NetPackSniff`)

## Usage

1. **Launch the application**
2. **Select a network interface** for capture
3. **Start capturing** packets using the "Start" button
4. **View and analyze** captured packets in the main table
5. **Apply filters** to focus on specific traffic
6. **Generate statistics** from the Statistics menu
7. **Save captures** for future reference using the Save option

## Supported Protocols

### Link Layer
- Ethernet

### Network Layer
- IPv4
- IPv6
- ARP
- ICMP

### Transport Layer
- TCP
- UDP

### Application Layer
- HTTP
- FTP
- SMTP
- POP3
- SSH
- Telnet

## Architecture

PacketLens follows a modular architecture with the following key components:

- **Packet Capture Engine**: Core component that interfaces with WinPcap/libpcap to capture packets
- **Protocol Analyzers**: Specialized modules for each supported protocol
- **Statistics Collection**: Modules that aggregate and visualize packet statistics
- **User Interface**: Java Swing-based interface for interaction and visualization

### Key Classes

- **NetPackSniff**: Main application class
- **Captor**: Manages packet capture sessions
- **PacketAnalyzer**: Base class for protocol analysis
- **StatisticsTaker**: Interface for statistics collection
- **Frame**: Main user interface window

## Requirements

### Minimum System Requirements
- **CPU**: 1 GHz or faster
- **RAM**: 512 MB
- **Disk Space**: 50 MB
- **Java**: JRE 8 or higher
- **Display**: 1024x768 resolution

### Recommended System Requirements
- **CPU**: 2 GHz dual-core or faster
- **RAM**: 2 GB or more
- **Disk Space**: 100 MB
- **Java**: JRE 11 or higher
- **Display**: 1920x1080 resolution

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

<div align="center">
  <p>
    <a href="https://github.com/VaibhavDaveDev/PacketLens/stargazers">⭐ Star this repo</a> •
    <a href="https://github.com/VaibhavDaveDev/PacketLens/issues/new">🐛 Report bug</a> •
    <a href="https://github.com/VaibhavDaveDev/PacketLens/issues/new">✨ Request feature</a>
  </p>
  <p>
    © 2025 <a href="https://github.com/VaibhavDaveDev">Vaibhav Dave</a>
  </p>
</div>
