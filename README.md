# LayerEight 🌐

> *Layer 8 is the human layer. We're building the AI that bridges human intent and network infrastructure.*

## What is LayerEight?

LayerEight is an open-source AI platform for network engineers, ISPs, and Internet Exchange Points built on a foundation model trained on the complete IETF RFC corpus — every internet standard ever published, from RFC 1 (1969) to present day.

Unlike general purpose AI tools, LayerEight starts from ground truth. Every recommendation, every config, every diagnosis is grounded in the actual standards the internet runs on.

## The Problem

Network engineers spend thousands of hours every year:
- Manually validating configs against RFC standards
- Interpreting cryptic syslog errors at 3am
- Writing boilerplate BGP configurations from scratch
- Chasing down misconfigurations that violate protocol standards

Existing tools are either vendor-locked, expensive, or not grounded in RFC truth.

## The Solution

A layered AI platform where every agent traces its knowledge back to RFC ground truth:
LayerEight Platform
│
├── RFC Foundation Model ← Qwen2.5-14B trained on 9,740 RFCs
│   Every internet standard from 1969 to present
│
├── Equipment Agents (in development)
│   ├── Juniper MX/QFX/PTX
│   ├── Cisco ASR/NCS/Nexus
│   ├── Nokia 7750 SR
│   ├── Arista 7500/7800
│   └── MikroTik CCR/CRS
│
├── Protocol Agents (planned)
│   ├── BGP Specialist
│   ├── OSPF/IS-IS Specialist
│   ├── MPLS/Segment Routing
│   └── Network Security
│
├── Operations Agents (planned)
│   ├── Error Analyzer — paste syslog, get RFC-cited diagnosis
│   ├── Config Generator — input parameters, get deployable config
│   ├── Config Validator — upload config, get RFC compliance report
│   └── Change Manager — predict impact before you deploy
│
└── Monitoring Agents (planned)
├── Real-time gNMI telemetry analysis
├── BGP hijack detection
├── Autonomous RFC compliance checking
└── Self-optimizing network management

## Models

| Model | Base | Training Data | Status |
|-------|------|---------------|--------|
| RFC-Qwen2.5-14B | Qwen2.5-14B-Instruct | 9,740 IETF RFCs | 🔄 Training |
| Juniper-14B | RFC-Qwen2.5-14B | Juniper TechLibrary | 📋 Planned |
| Cisco-14B | RFC-Qwen2.5-14B | Cisco Documentation | 📋 Planned |
| Nokia-14B | RFC-Qwen2.5-14B | Nokia Documentation | 📋 Planned |
| BGP-Agent | RFC-Qwen2.5-14B | BGP RFCs + NANOG | 📋 Planned |
| Error-Analyzer | All above | Syslog + TAC cases | 📋 Planned |

## Hugging Face

Models are published at [LayerEight on Hugging Face](https://huggingface.co/LayerEight)

## Hardware

This project proves that serious AI training is possible on consumer AMD hardware:

- **GPU**: AMD Radeon RX 9070 XT (16GB VRAM)
- **Framework**: PyTorch 2.11.0 + ROCm 7.2
- **Training**: QLoRA 4-bit quantization via bitsandbytes
- **Platform**: WSL2 on Windows 11

If it runs on a 9070 XT it runs on anything.

## Use Cases

**For IXP Operators:**
- Route server configuration generation
- Peering policy validation
- BGP community planning
- RFC 7454 (BGP Operations and Security) compliance checking

**For ISPs:**
- Transit routing configuration
- Customer BGP session templates
- IP address management
- MPLS traffic engineering

**For Network Engineers:**
- Paste a syslog error → get RFC-cited diagnosis
- Describe your network → get deployable config
- Upload existing config → get compliance report

**For Students:**
- RFC-grounded explanations of every protocol
- CCNA/CCNP/JNCIA study assistance
- Lab configuration help
- Real standard citations not just exam dumps

## Roadmap

- [x] Phase 1: RFC Foundation Model (training now)
- [ ] Phase 2: Juniper Equipment Model
- [ ] Phase 3: Cisco Equipment Model  
- [ ] Phase 4: BGP Protocol Specialist
- [ ] Phase 5: Error Analyzer Agent
- [ ] Phase 6: Config Generator
- [ ] Phase 7: Real-time Network Monitor
- [ ] Phase 8: Full Orchestrator — unified LayerEight platform

## Contributing

This project welcomes contributions from the networking community:
- Training data (anonymized configs, error logs)
- RFC dataset improvements
- Vendor documentation datasets
- Testing and validation
- Documentation

## License

Apache 2.0 — open source, free to use, free to build on.

## About

Built by a network infrastructure developer in Jeffersonville, Indiana.
Trained on AMD RDNA4 hardware because if it works on the hard platform,
it works everywhere.

*"Layer 8 is the human layer. We're building the AI that sits between
the human and the network."*
