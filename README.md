# Network Latency and Packet Loss Chaos Emulator

A Linux Kernel Module (LKM) based network fault injection tool designed to emulate network turbulence, including packet latency, packet loss, and UDP payload corruption directly within the Linux network stack.

---

## Features
- **Linux Kernel Driver:** Uses Netfilter hooks (`NF_INET_PRE_ROUTING`) for packet interception.
- **IPC Architecture:** Uses IOCTL (`/dev/chaos_emulator`) to communicate with the C++ control program.
- **Latency Injection:** Configurable packet delay simulation.
- **Packet Loss:** Probabilistic packet dropping mechanism.
- **Payload Corruption:** Targeted bit-flipping on UDP packet payloads.

---

## Requirements
- Linux OS (Ubuntu / Debian)
- `gcc`, `g++`, `make`, and Kernel Headers

---

## How to Build and Run

### 1. Compile the project
```bash
make
