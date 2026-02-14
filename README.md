# R.G. Lefever

Four decades of building software. Currently: four open-source ecosystems, one coherent stack, zero compromises.

## About

Started on a ZX81 in the early 80s. Went professional in the early 90s. Forty years later, I'm still writing code — I just got considerably better at knowing what not to write.

I build event-sourced, distributed systems in Erlang/OTP, with Rust where speed matters and Go where humans have to look at it. Most people reach for a database and a framework. I built both, then built a network layer, then built a developer studio on top. Then I taught neural networks to evolve themselves.

Based in Leuven, Belgium. Working through [DisComCo sp.z.o.o](https://discomco.pl). Ham radio callsign SP8RL.

## What I'm Building

### ReckonDB

Because the BEAM deserved its own event store. Built on Khepri/Ra with Raft consensus — a complete CQRS/Event Sourcing stack: the event store itself, a CQRS framework (evoq), and an adapter layer that connects them. Optional Rust NIFs for high-performance cryptography and compression. No external database dependencies. No compromises.

**Erlang, Rust, Khepri/Ra, SQLite** | [reckon-db-org](https://github.com/reckon-db-org) | 17 repos

### Macula

HTTP/3 mesh networking platform for decentralized applications. Nodes form self-organizing networks using Kademlia DHT routing, QUIC transport for NAT traversal, and content-addressed distribution. Designed for edge and resource-constrained environments. Masterless consistency via CRDTs, capability-based security with DID identities and UCAN tokens.

**Erlang, MsQuic/HTTP3, Kademlia, CRDTs** | [macula-io](https://github.com/macula-io) | 34 repos

### Hecate

AI-powered developer studio. An Erlang daemon handles event sourcing, mesh integration, and multi-provider LLM orchestration (Ollama, OpenAI, Anthropic, Google). A Go terminal UI provides the developer experience: chat, code exploration, project management, and mesh-connected agent coordination.

**Erlang, Go, Bubble Tea, Multi-LLM** | [hecate-social](https://github.com/hecate-social) | 12 repos

### Faber

Neuroevolution on the BEAM. A TWEANN engine with Liquid Time-Constant neurons that evolve their own topology and weights. Population-based training, multi-objective fitness, speciation — neural networks that design themselves. Optional Rust NIFs for 10-200x acceleration. Built on Gene Sher's DXNN2 research, rewritten from scratch.

*Faber: Latin for maker. It's been my name the whole time.*

**Erlang, Rust NIFs, Mnesia, NEAT/TWEANN** | [rgfaber](https://github.com/rgfaber) | 6 repos

## The Stack

```
  Hecate        developer experience, AI agents
    |
  Macula        mesh networking, P2P distribution
    |       \
  ReckonDB   Faber       event sourcing / neuroevolution
```

ReckonDB provides the event sourcing infrastructure that both Macula and Hecate build on. Macula provides the distributed network layer that Hecate uses to connect developer agents across nodes. Hecate is the interface layer where developers interact with the whole stack. Faber provides the computational intelligence — neural networks that evolve on the BEAM, optionally distributed across the Macula mesh.

Each ecosystem stands on its own. Together they form a vertically integrated platform for building distributed, event-sourced, AI-assisted applications on the BEAM. 69 repos across 4 ecosystems, spanning Erlang, Rust, Go, and Svelte. One person, one vision.

## Links

- [Blog](https://discomco.pl)
- [GitHub](https://github.com/rgfaber)
- [Support my work](https://buymeacoffee.com/rlefever)
