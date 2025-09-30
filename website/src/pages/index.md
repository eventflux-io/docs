# EventFlux Documentation

## What is EventFlux?

EventFlux is a **pattern-first stream processing engine (CEP)** built in Rust. It is designed for teams who need real-time computation without the complexity of a full streaming platform.

EventFlux enables you to compose filters, maps, joins, enrichment, windows, and temporal patterns, then execute them in milliseconds on-prem or in Kubernetes. With predictable performance, straightforward operations, and extensible connectors, EventFlux delivers the essentials of real-time computation—without platform lock-in or broker overhead.

## The Name

**Event**: We compute over events (not a broker/platform).

**Flux**: Continuous movement—data in motion, responsive by design.

## Core Capabilities

EventFlux provides essential stream processing capabilities:

- **Filters, maps, projections** — Transform and filter event streams
- **Stateful and stateless operators** — Build complex processing pipelines
- **Stream-to-table and stream-to-stream joins** — Combine data from multiple sources
- **Enrichment via external stores and caches** — Add context to events in real-time
- **Windows and watermarking** — Tumbling, sliding, and session windows with late-data handling
- **CEP patterns** — Sequence detection, absence patterns, correlation, and time-bounded triggers
- **Connectors** — Extensible integration with common sources and sinks
- **Delivery guarantees** — Exactly-once and at-least-once modes (where supported)
- **Observability** — Metrics and tracing hooks for monitoring

## Key Characteristics

### Pattern-First by Design

Complex event patterns (sequences, absence, correlation) are built into the engine—not bolted on.

### Rust-Fast, Predictable Latency

Consistent performance with a small footprint, ideal for edge and on-prem deployments. No GC pauses or long warmups.

### Essential, Not Excessive

The stream processing you need—filters, joins, enrichment, windows—without platform bloat.

### Operate Anywhere

Clean self-hosted experience with Kubernetes-friendly deployment options.

### Composable & Extensible

Connectors for common sources and sinks. Pipelines are made of clear, reusable operators.

## Who Uses EventFlux?

EventFlux is designed for:

- **Platform and infrastructure teams** that need real-time computing without running a full streaming platform
- **Fraud, risk, and security teams** that require pattern detection and correlation
- **Observability and SRE teams** correlating events across services and time windows
- **IoT and telemetry teams** processing sensor data with enrichment at the edge

## Technology

EventFlux is built in **Rust**, providing:

- **Predictable latency** with no garbage collection pauses
- **Memory safety** with low overhead
- **Small binaries and fast startup times**
- **Edge and on-prem friendly** operations

## Coming Soon

EventFlux is currently under development. This documentation site will be populated with comprehensive guides, API references, and deployment instructions as the project progresses toward its 1.0 release.

## Get Involved

Visit [eventflux.io](https://eventflux.io) for more information and updates.
