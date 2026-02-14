# R.G. Lefever

I build distributed systems on the BEAM. Three open-source ecosystems, one coherent stack.

## About

I've been writing code since the early 80s (ZX81) and professionally since the early 90s. My focus is event-sourced, distributed systems built primarily in Erlang/OTP, with Rust for performance-critical paths and Go for developer tooling.

I work through [DisComCo sp.z.o.o](https://discomco.pl) from Leuven, Belgium. Ham radio callsign SP8RL.

## What I'm Building

### ReckonDB

BEAM-native distributed event store built on Khepri/Ra with Raft consensus. A complete CQRS/Event Sourcing stack: the event store itself, a CQRS framework (evoq), and an adapter layer that connects them. Optional Rust NIFs for high-performance cryptography and compression. No external database dependencies.

**Erlang, Rust, Khepri/Ra, SQLite** | [reckon-db-org](https://github.com/reckon-db-org) | 17 repos

### Macula

HTTP/3 mesh networking platform for decentralized applications. Nodes form self-organizing networks using Kademlia DHT routing, QUIC transport for NAT traversal, and content-addressed distribution. Designed for edge and resource-constrained environments. Masterless consistency via CRDTs, capability-based security with DID identities and UCAN tokens.

**Erlang, MsQuic/HTTP3, Kademlia, CRDTs** | [macula-io](https://github.com/macula-io) | 34 repos

### Hecate

AI-powered developer studio. An Erlang daemon handles event sourcing, mesh integration, and multi-provider LLM orchestration (Ollama, OpenAI, Anthropic, Google). A Go terminal UI provides the developer experience: chat, code exploration, project management, and mesh-connected agent coordination.

**Erlang, Go, Bubble Tea, Multi-LLM** | [hecate-social](https://github.com/hecate-social) | 12 repos

## The Stack

```
  Hecate        developer experience, AI agents
    |
  Macula        mesh networking, P2P distribution
    |
  ReckonDB      event sourcing, CQRS, persistence
```

ReckonDB provides the event sourcing infrastructure that both Macula and Hecate build on. Macula provides the distributed network layer that Hecate uses to connect developer agents across nodes. Hecate is the interface layer where developers interact with the whole stack.

Each ecosystem stands on its own. Together they form a vertically integrated platform for building distributed, event-sourced, AI-assisted applications on the BEAM.

## Links

- [Blog](https://discomco.pl)
- [GitHub](https://github.com/rgfaber)
- [Support my work](https://buymeacoffee.com/rlefever)
