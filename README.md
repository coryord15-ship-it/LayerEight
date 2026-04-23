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

A layered AI platform where every agent traces its knowledge back to RFC ground truth.

**Layer 1 — RFC Foundation Model** — training now on 9,740 IETF RFCs from 1969 to present. The ground truth everything else builds on.

**Layer 2 — Equipment Agents** — vendor specific models built on top of the RFC foundation. Juniper, Cisco, Nokia, Arista, MikroTik.

**Layer 3 — Protocol Agents** — BGP specialist, OSPF/IS-IS specialist, MPLS/Segment Routing, Network Security.

**Layer 4 — Operations Agents** — Error Analyzer, Config Generator, Config Validator, Change Manager.

**Layer 5 — Monitoring Agents** — real time gNMI telemetry, BGP hijack detection, autonomous RFC compliance, self optimizing network management.

**Layer 6 — Orchestrator** — unified interface that routes to all agents and combines answers into single RFC-cited responses.
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

Models published at [LayerEight on Hugging Face](https://huggingface.co/LayerEight)

## Hardware

- **GPU**: AMD Radeon RX 9070 XT (16GB VRAM)
- **Framework**: PyTorch 2.11.0 + ROCm 7.2
- **Training**: QLoRA 4-bit via bitsandbytes
- **Platform**: WSL2 on Windows 11

If it runs on a 9070 XT it runs on anything.
## Use Cases

**For IXP Operators**
- Route server configuration generation
- Peering policy validation
- BGP community planning
- RFC 7454 compliance checking

**For ISPs**
- Transit routing configuration
- Customer BGP session templates
- MPLS traffic engineering

**For Network Engineers**
- Paste syslog error and get RFC-cited diagnosis
- Describe your network and get deployable config
- Upload config and get compliance report

**For Students**
- RFC-grounded protocol explanations
- CCNA/CCNP/JNCIA study help
- Real standard citations not exam dumps

## Roadmap

- [x] Phase 1: RFC Foundation Model
- [ ] Phase 2: Juniper Equipment Model
- [ ] Phase 3: Cisco Equipment Model
- [ ] Phase 4: BGP Protocol Specialist
- [ ] Phase 5: Error Analyzer Agent
- [ ] Phase 6: Config Generator
- [ ] Phase 7: Real-time Network Monitor
- [ ] Phase 8: Full LayerEight Orchestrator

## Contributing

- Training data (anonymized configs, error logs)
- RFC dataset improvements
- Vendor documentation datasets
- Testing and validation

## License

Apache 2.0

## About

Built by a network infrastructure developer in Jeffersonville, Indiana.
Trained on AMD RDNA4 hardware because if it works on the hard platform it works everywhere.

*"Layer 8 is the human layer. We're building the AI that sits between the human and the network."*
