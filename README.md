-------
| REPO LINKS |
|----- |
| [MAMAWMAIL RESEARCH INITIATIVE](https://github.com/Mamawmail-Research-Initiative) : Github Organization  |
| [Intelligent Fractal Propagation Protocol](https://github.com/juancarlosayeng/mamawmail-intelligent-fractal-propagation-protocol-whitepaper) : IFPP Whitepaper  |
| [Mamawmail SYSTEM Whitepaper](https://github.com/juancarlosayeng/mamawmail-system-whitepaper) : IFPP Implementation/Application Whitepaper  |
| [Mamawmail](https://github.com/juancarlosayeng/mamawmail) : IFPP Implementation  |
-------
UPDATED: October 28 2025

# IFPP + MAMAWMAIL WHITEPAPER STRUCTURE [Current Version] 

 
1. [x] [Intelligent Fractal Propagation Protocol Whitepaper](https://github.com/juancarlosayeng/mamawmail-intelligent-fractal-propagation-protocol-whitepaper/blob/main/docs/The%20Intelligent%20Fractal%20Propagation%20Protocol%20(IFPP)%20A%20Protocol%20Originating%20from%20the%20MAMAWMAIL%20Project%20Whitepaper%20%E2%80%94%20September%2022%202025%20-%20Engr%20Juan%20Carlos%20G%20Ayeng%20-%20Bacolod%20City%20-%20Philippines.pdf) 
   1. [x] Annex A [IFPP MESSAGE PACKET SPECIFICATION AND STATELESS TRANSPORT BEHAVIOR](https://github.com/juancarlosayeng/mamawmail-intelligent-fractal-propagation-protocol-whitepaper/blob/main/docs/ANNEX%20A%20-%20The%20Intelligent%20Fractal%20Propagation%20Protocol%20IFPP%20A%20Protocol%20Originating%20from%20the%20MAMAWMAIL%20Project%20Whitepaper%20%E2%80%94October%2015%202025%20-%20Engr%20Juan%20Carlos%20G%20Ayeng%20-%20Bacolod%20City%20-%20Philippines.pdf)
   2. [ ] Annex B - ONGOING - [IFPP PHYSICAL TRANSFER AND CARRIER LAYER EXPRESSIONS](https://github.com/juancarlosayeng/mamawmail/blob/main/docs/Annex_B-IFPP_Physical_Transfer_and_Carrier_Layer_Expressions.md)
   3. [ ] Annex C - ONGOING - <b>Archangel Gabriel [AI]: Swarm Supra-Entity and Integrity Sentinel</b> 
  
      
2. [ ] Mamawmail Whitepaper - [ONOING/Unfinished](https://github.com/juancarlosayeng/mamawmail-intelligent-fractal-propagation-protocol-whitepaper/blob/main/docs/MAMAWMAIL%20-%20%20A%20Decentralized%20Communication%20System%20Updated%20Whitepaper%20%E2%80%94%20September%2027%202025%20(Original%20June%2020%202025)%20-%20Engr%20Juan%20Carlos%20G%20Ayeng%20-%20Bacolod%20City%20-%20Philippines.docx)

 <br><br><br>
 SAMPLE ONGOING RESEARCH - adding more annexes, sections and research
## ANNEX-B Table: Projected Computational and Transmission Costs

This section quantifies the expected energy, storage, and bandwidth requirements during a full IFPP hop cycle between two devices.
The estimates are based on current-generation mobile hardware (ARM A53–A76 class CPUs, 4 GB RAM, 10 MB/s equivalent link) and optimized cryptographic operations (SHA3–256 and XChaCha20-Poly1305).
Values are averages designed for modeling and comparative evaluation with TCP/IP message delivery.
 <br>
| Stage                         | Description                                 | Device A (Sender)                                            | Device B (Receiver)    | Typical Duration | Notes                            |
|-------------------------------|---------------------------------------------|--------------------------------------------------------------|------------------------|------------------|----------------------------------|
| 1 – Payload Receipt           | App → Team Leader message load              |    8 KB RAM, 0.3 MB I/O                                      | -                      | 1ms              | No crypto; memory copy only      |
| 2 – Intel ↔ Gabriel           |    Candidate discovery, AI digest   sync    | 0.5 KB TX / 1 KB RX (≈1.5 KB total)                          | 0.5 KB RX / 1 KB TX    | 2–5 ms           |    Short JSON digest exchange    |
| 3 – Liaison Device Engagement | Candidate signal probe                      | < 2 KB RF signal frames                                      | 2 KB probe response    | 3-7 ms           | BLE/Wi-Fi beacon or UDP ping     |
| 4 – Point Binding             | Object binding + hash computation           | 32 KB RAM (SHA3) ≈ 2 ms CPU                                  | -                      | 2 ms             | 0.002 Wh compute cost            |
| 5 – Heavy Weapons Security    | Security update & verification              | 1 MB read + 64 KB write (≈2 MB I/O)                          | -                      | 15-25 ms         | Most expensive CPU stage (8%)    |
| 6 – Pre-Interaction Sync      | Angel team coordination                     | 128 KB RAM                                                   | 128 KB RAM             | 1 ms             | Negligible bandwidth             |
| 7 – Candidate Evaluation      | 3-node scoring and prioritization           |    1.5 MB RAM compute                                        | -                      | 5 ms             | Local AI inference vectorization |
| 8 – Recon Scouting            | Probe and verification on 3 targets         | 3 × 512 B TX                                                 | 3 × 512 B RX           | 8 ms             | Maintains micro-links            |
|    9 – Hop Decision           | Team Leader + Gabriel evaluation            | 64 KB RAM                                                    | -                      | <1 ms            | Decision matrix merge            |
| 10 – Security Instantiation   | Pre-arrival sandbox deploy                  | -                                                            | 0.5 MB disk write      | 5 ms             | Security sweep initialization    |
| 11 – Message Transfer         | Three-burst transmission                    | 2 KB (Ephemeral) + 4 KB (Metadata) + 10 KB (Core) = 16 KB TX | 16 KB RX               | 1-2 ms           | One-shot burst; no ACK cycle     |
| 12 – Post-Hop Deploy          | Angel re-spawn logic                        | 16 KB RAM                                                    | 32 KB RAM              | 2ms              | Code copy + hash verify          |
| 13 – Hop Confirm ↔ Gabriel    |    Hop status confirmation                  | 1 KB TX / RX                                                 | 1 KB TX / RX           | 1 ms             | Swarm ledger update              |
| 14 – All-Clear Signal         | Passive Gabriel confirmation                | -                                                            | < 0.1 KB RX            | Variable         | Triggered remotely               |
| 15 – Self-Deletion            | Memory release and cleanup                  |    32 KB RAM                                                 | -                      | 0.5 ms           | Garbage collection event         |
| 16 – Cycle Re-Instantiation   | Angel reload on next device                 | -                                                            | 64 KB RAM + 0.5 MB I/O | 2 ms             | Fresh process spawn              |


### Aggregate Resource Cost per Hop (One Device Pair)
| Metric                                         | Device A (Sender) | Device B (Receiver) |     Combined Total     |
|------------------------------------------------|-------------------|---------------------|------------------------|
|    Storage footprint (volatile + temp disk)    | ≈ 2.8 MB          | ≈ 1.1 MB            |    ≈ 3.9 MB            |
| Bandwidth usage (TX + RX combined)             | ≈ 25 KB           | ≈ 25 KB             | ≈ 50 KB per hop        |
| Energy draw                                    | ≈ 0.07 Wh         | ≈ 0.05 Wh           |    ≈ 0.12 Wh total     |
| Compute time (active CPU)                      | ≈ 70 ms           | ≈ 40 ms             | ≈ 110 ms total         |

<br><br><br><br>
## TCP/IP Transmission Baseline (10 KB Payload Example)
| Stage                    | Process                              | Device A (Sender) | Device B (Receiver) | Typical Duration |
|--------------------------|--------------------------------------|-------------------|---------------------|------------------|
| 1 – 3-Way Handshake      | SYN, SYN-ACK, ACK (3 packets × 60 B) | 180 B TX/RX       | 180 B TX/RX         | 15–30 ms         |
| 2 – TLS Handshake        | ECDHE + Certificate exchange         | 4 KB TX + 4 KB RX | 4 KB TX + 4 KB RX   | 120–200 ms       |
| 3 – Payload Transmission | 10.5 KB TX                           | 10.5 KB RX        | 10–20 ms            |                  |
| 4 – ACK & Keepalive      | 1 KB TX / RX                         | 1 KB TX / RX      | 5 ms                |                  |
| 5 – Session Close        | 0.5 KB TX / RX                       | 0.5 KB TX / RX    | 5 ms                |                  |

### Aggregate Cost (10 KB TCP Payload)
| Metric                             | Device A (Sender) | Device B (Receiver) |     Combined Total     |
|------------------------------------|-------------------|---------------------|------------------------|
| Bandwidth usage (over the air)     | 25 KB             | 25 KB               | ≈ 50 KB total          |
| Bandwidth usage (TX + RX combined) | 150–260 ms        | -                   | ≈ 200 ms average       |
| Energy draw                        | ≈ 0.30 Wh         | ≈ 0.25 Wh           | ≈ 0.55 Wh total        |
| Socket duration                    | 250 ms            | 250 ms              | -                      |

### Analytical Comparison
| Category           | IFPP [Per Hop]             | TCP/IP [10kb Message] | Relative Efficiency               |
|--------------------|----------------------------|-----------------------|-----------------------------------|
| Storage (volatile) | 3.9 MB                     | 4.0 MB                | ≈ Parity                          |
| Energy Draw        | 0.12 Wh                    | 0.55 Wh               | 4.5× more efficient               |
| Latency            | 110 ms                     | 200 ms                | ≈ 2× faster                       |
| Bandwidth          | 50 KB                      | 50 KB                 | Equal (IFPP includes AI metadata) |
| Security Overhead  | Self-authenticating digest | TLS cert chain        | ≈ 80% lighter                     |

<br>

## Interpretive Commentary  

### Compute Efficiency:
> IFPP’s event-driven architecture replaces persistent sockets with short-lived microtransactions, cutting power consumption by up to 75%.  

### Reduced Latency:
> Hop decisions overlap with Gabriel synchronization, enabling sub-100 ms behavior within three-hop swarm radius.  

### Stable Memory Pressure:  
> Because each angelic module self-deletes post-hop, per-device memory load remains constant even during heavy network churn.

### Security Simplicity:
> Eliminates TLS certificate dependencies — authentication occurs directly through device key digests.  

### Scalability Trend:
> As devices adopt multi-core AI accelerators (ARMv9 / RISC-V), IFPP’s efficiency gains scale sub-linearly with hop count, meaning greater network size yields higher relative throughput per watt.


<br><br><br><br>
<hr>
<br><br><br><br>
UPDATED: October 14 2025

🧩 New Annex Added 

Annex A — IFPP Message Packet Specification and Stateless Transport Behavior
Defines the three-part IFPP message structure (Ephemeral Header, AI Metadata, Eternal Message Core) and outlines stateless, no-socket transport modes via UDP, Bluetooth, Wi-Fi, and TCP/IP bridge.

📘 Preview:
“Each IFPP message is composed of three interdependent yet independently storable components:
— Ephemeral Header – transient bootstrap and authentication data.
— AI Metadata – dynamic, self-evolving contextual information for learning and traceability.
— Eternal Message Core – immutable encrypted payload representing the true message.”


<details>
<summary>🧩 Annex A — IFPP Message Packet Specification and Stateless Transport Behavior</summary>

> Defines the three-part IFPP message structure (Ephemeral Header, AI Metadata, Eternal Message Core).  
>  
> 🔗 [Read Full Annex A (Markdown)](docs/Annex_A-IFPP_Message_Packet_Specification_and_Stateless_Transport_Behavior_Beta_102025.md)  
> 📄 [Download PDF Version](docs/Annex_A-IFPP_Message_Packet_Specification_and_Stateless_Transport_Behavior_Beta_102025.pdf)

</details>

<hr>


UPDATED: October 1 2025

# Submitted New IFPP Whitepaper to NLNET. 
- Separated IFPP from Mamawmail into its own Whitepaper.
<br><br>
- Github Repo about to be updated after finishing Mawmawmail Whitepaper.
<br><br>

-----------------------------------------------------


UPDATED: August 24 2025

Part of the Mamawmail Research Initiative – theoretical foundation of IFPP.
-----------------------------------------------------
## Mamawmail Research Initiative – License Overview

The Mamawmail Research Initiative is a combined effort of theoretical research,  
system architecture design, and practical software implementation.  

It is organized into three connected repositories, each with its own license.  
The whitepapers provide the **research foundation** and theoretical framework,  
while the implementation repository translates those ideas into a working system.  

| Repository                                                | License                              | Purpose                                                   |
| --------------------------------------------------------- | ------------------------------------ | --------------------------------------------------------- |
| **mamawmail-intelligent-propagation-protocol-whitepaper** | CC BY-SA 4.0 (open research license) | Formal description of the Intelligent Fractal Propagation Protocol (IFPP), mathematical models, and comparisons |
| **mamawmail-system-whitepaper**                           | AGPL-3.0 (Community) + Commercial    | Broader system design, AI integrations, and saturation singularity theory |
| **mamawmail**                                             | AGPL-3.0 (Community) + Commercial    | Practical implementation of the Mamawmail system (Community & Enterprise editions) |

<br><br><br><br>
--------------------------------------------------




# mamawmail-intelligent-propagation-protocol-whitepaper
Core research and development repository for the Mamawmail system – a decentralized, intelligent fractal propagation protocol (IFPP) for peer-to-peer communication.  Contains formal documentation, simulations, and mathematical models for message propagation, delivery assurance, and network resilience.


## Contents
- Whitepaper drafts  
- Mathematical models  
- Simulation data  
- Research notes  

## License
This repository is licensed under the **Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)**.  
See the [LICENSE](LICENSE) file for details.

----------------------------------------

# Intelligent Fractal Propagation Protocol (IFPP)

👋 Welcome!  
This repository is dedicated to the **Intelligent Fractal Propagation Protocol (IFPP)** — the "engine" behind **Mamawmail**.

---

## Why a Separate Repository?

We’ve chosen to separate the work into **three focused repositories**:

1. **IFPP** (this repo) –  
   The **core innovation**: math, proofs, comparisons with other protocols, and open simulations.  
   Think of it as the **engine** that shows *why* this protocol is different.

2. **Mamawmail-Whitepaper** –  
   The **system-wide vision**: AI federated learning, propagation singularities, and the broader architecture.  
   Think of it as the **blueprint of the car**.

3. **Mamawmail (Implementation)** –  
   The **working application**: community edition, enterprise modules, and integration code.  
   Think of it as the **car itself**, with parts you can drive, extend, and commercialize.

This structure avoids confusion and makes it easier for evaluators, implementers, and researchers to **focus on what matters to them**.

---

## What You’ll Find Here

- 📘 **Formal Papers** – structured protocol descriptions following existing research standards.  
- ➗ **Mathematics** – equations, models, and derivations behind IFPP.  
- 📊 **Comparisons** – side-by-side analysis with Email, DTN, Gossip, Spray-and-Wait, and others.  
- 🎥 **Animations & Simulations** – Python templates and visualizations that make IFPP’s behavior *visible*.  
- 📚 **References & Glossary** – to align with existing work and terminology.

---

## Who Is This Repo For?

- **Researchers** – who want to study, verify, or build upon the IFPP protocol.  
- **Implementers** – who want ready-to-use templates for simulations.  
- **Evaluators** – who want to clearly see how IFPP differs from traditional protocols.  
- **Contributors** – who want to improve models, proofs, or visualizations.

---

## Final Note

This repo is not the *entire system*.  
It is **focused deliberately on the "engine"** — where innovations can be highlighted and compared transparently.  
If you’re curious about the **whole vehicle**, please see:  
- [Mamawmail-Whitepaper](link-to-whitepaper-repo)  
- [Mamawmail Implementation](link-to-implementation-repo)  

Together, these three repositories form the complete vision of a decentralized, intelligent, and resilient communication system.

---

🔑 License: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)  
Contributions and forks are welcome, as long as proper attribution is given and knowledge remains open.
