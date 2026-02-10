<img width="1398" height="1556" alt="generated-image(1)" src="https://github.com/user-attachments/assets/f32d21a0-33d0-41f5-a13b-0c8b9e31d400" />

[![Kotlin](https://img.shields.io/badge/Kotlin-red)](https://kotlinlang.org/)
[![JRuby](https://img.shields.io/badge/JRuby-red)](https://www.jruby.org/)

## **⚠️ LEGAL DISCLAIMER**
**DroidXploit** is a powerful penetration testing framework designed for **security researchers, ethical hackers, and authorized security assessments**. This app must only be used on networks and systems you **own or have explicit written permission** to test.

**UNAUTHORIZED USE IS ILLEGAL AND PUNISHABLE BY LAW.**

The developers assume **NO RESPONSIBILITY** for misuse, damage, or illegal activities performed with this tool.

🔥 **Features**

📱 **Module Management**

✅ Dynamic .rb Module Loading - Import Ruby-based exploits (with limitations)
✅ Multiple Module Types - Exploit, Auxiliary, Payload, Post, Encoder
✅ Hot-Reload Modules - Update exploits without restarting
✅ Module Filtering - Search and filter by type, name, or CVE
✅ Auto-Parse Metadata - Extracts name, author, description from .rb files

🔧 **Module Compatibility**

**Native Support (No Adaptation Required)**

Most Metasploit modules using basic TCP/UDP work directly without modification:

✅ **Works Out-of-the-Box (~50% of modules)**
    - TCP-based modules - SSH/FTP/Telnet brute force, port scanners
    - UDP-based modules - DNS attacks, basic UDP exploits
    - Scanner modules - Service detection, bannergrabbing
    - Simple DoS - Application-layer attacks

**Adaptation Required (Mixin Substitution + Manual Protocol Encoding)**

Complex protocol modules need manual adaptation (~30% of modules):

⚙️ **Requires Adaptation**
    - SNMP modules - Replace SNMPClient with Udp + manual ASN.1/BER encoding
    - SMB modules - Replace SMB with Tcp + custom packet structures
    - Complex HTTP - May need manual header/body construction
    - Custom protocols - Implement packet encoding from scratch

💉 **Exploitation Capabilities**

✅ Network Protocols (NATIVE SUPPORT)
- TCP Socket Attacks - SSH/FTP brute force, Telnet exploits
- UDP Exploits - Raw packet injection, DNS attacks
- Port Scanning - TCP connect scan, service detection
- Protocol Fuzzing - Basic network fuzzing

⚙️ **Protocols (ADAPTATION REQUIRED)**
- SNMP - Manual ASN.1/BER encoding via UDP
- SMB/NetBIOS - Custom packet construction via TCP
- Complex HTTP - Manual header/body formatting may be needed

⚠️ **Limited Support (Partial Functionality)**
- DoS Attacks - Application-layer works, network-layer requires ROOT
- SSL/TLS Attacks - Certificate validation bypass works

❌ NOT SUPPORTED (Requires ROOT, Native Code, or Major Rework)
- Raw Socket Attacks - SYN flood, ARP spoofing, ICMP flood
- Packet Crafting - Custom TCP/IP headers manipulation
- Wireless Attacks - WiFi deauth, WPA cracking
- Meterpreter Payloads - Full Metasploit Framework required
- Post-Exploitation - Session management, pivoting, routing
- Platform-Specific - Windows Registry, WMI, PowerShell modules

🖥️ **Console Interface**

✅ Interactive Terminal - Metasploit-like command interface
✅ Real-Time Output - Live exploitation feedback
✅ Module Configuration - Set RHOST, RPORT, COMMUNITY and custom options
✅ Command History - Navigate previous commands
✅ Auto-Completion - Common commands and module names

🎨 **User Interface**

✅ Material Design 3 - Modern, dark-themed interface
✅ Ruby Red Accent - Aggressive, hacker-inspired color scheme
✅ Module Cards - Visual module organization with type badges
✅ Statistics Dashboard - Track loaded modules by type
✅ Progress Indicators - Real-time import/execution status

⚠️ **Compatibility Notes**

**Tested & Verified:**
- ✅ TCP socket operations (confirmed via network tests)
- ✅ UDP socket operations (confirmed via DNS tests)
- ✅ Basic Metasploit module structure compatibility

**Estimated Compatibility:**
- Module adaptation success rates are based on Metasploit framework analysis
- Actual results may vary depending on module complexity
- Test modules in a safe environment before production use

**Not all Metasploit modules will work without modification.** Check module dependencies before loading.
