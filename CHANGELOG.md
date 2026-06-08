# Changelog

All notable changes to this project are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [1.1.0] - 2026-06-07

### Added
- **SOAP archetype** — Full coverage of Simple Object Access Protocol:
  - *"The Royal Notary Guild"* analogy explaining the contract-first, envelope-wrapped model
  - Step-by-step breakdown of WSDL, XML envelopes, SOAP Faults, and WS-* extensions
  - Python server example using `spyne`
  - Python client example using `zeep`
  - Node.js client example using the `soap` package with raw XML envelope shown
  - SOAP column added to the full comparison matrix
  - SOAP entry in the Quick Decision Map and Architect's Heuristics
- `SECURITY.md` — responsible disclosure policy and production security guidance for code examples
- `CONTRIBUTING.md` — guide for adding archetypes, fixing examples, and UI improvements
- `SUPPORT.md` — help resources, FAQ, and learning path for students

---

## [1.0.0] - 2026-06-07

### Added
- Initial release of the **API Archetypes Field Guide**
- Six API archetypes with full detail pages:
  - **REST** — *"The Royal Postal System"* (FastAPI server, httpx + fetch clients)
  - **GraphQL** — *"The Oracle of Delphi"* (Strawberry + FastAPI server)
  - **gRPC** — *"The Legion's Signal Corps"* (Protocol Buffers + grpc)
  - **WebSocket** — *"The Palantir Network"* (FastAPI + asyncio + browser WS API)
  - **Webhook** — *"The Raven Network"* (HMAC-signed event delivery, retry logic)
  - **SSE** — *"The Town Crier"* (Server-Sent Events with EventSource)
- Full comparison matrix across 10 production-relevant dimensions
- Quick Decision Map for at-a-glance architecture decisions
- Architect's Heuristics panel with one rule per archetype
- Three code tabs per archetype: Python server · Python client · JavaScript client
- Copy-to-clipboard button on all code blocks
- Dark theme UI with per-archetype color coding and fantasy glyphs
- MIT License
