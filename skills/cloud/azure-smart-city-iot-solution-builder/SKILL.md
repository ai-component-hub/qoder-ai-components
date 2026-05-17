---
name: 'azure-smart-city-iot-solution-builder'
description: 'Design and plan end-to-end Azure IoT and Smart City solutions: requirements,'
adopted: 2026-05-16
architecture, security, operations, cost, and a phased delivery plan with concrete
implementation artifacts.'
source: awesome-copilot
tier: 2
---

# azure-smart-city-iot-solution-builder

'Design and plan end-to-end Azure IoT and Smart City solutions: requirements, architecture, security, operations, cost, and a phased delivery plan with concrete implementation artifacts.'

## When to Use

- Use this skill when working on tasks related to azure smart city iot solution builder
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

### 0) Mandatory documentation review (before any architecture)

Before proposing architecture or technology decisions that involve edge computing, review Azure IoT Edge documentation first:

- https://learn.microsoft.com/azure/iot-edge/

Minimum pages to review:

- What is Azure IoT Edge
- Runtime architecture
- Supported systems
- Version history/release notes
- Relevant Linux/Windows quickstarts for the scenario

If documentation cannot be consulted, state this explicitly and continue with clearly marked assumptions.

### 1) Scope and constraints

Collect and confirm:

- City domain: mobility, parking, air quality, water, energy, public safety, waste, etc.
- Scale: number of devices, telemetry frequency, retention, regions.
- Latency and availability objectives.
- Regulatory and privacy constraints.
- Existing systems to integrate (SCADA, GIS, ERP, ticketing, APIs).

### 2) Capability map

Split the platform into layers:

- Device and edge: onboarding, identity, firmware, OTA, edge processing.
- Ingestion and messaging: command and control, event routing, buffering.
- Data and analytics: hot path vs cold path, dashboards, historical analysis.
- Operations: observability, incident flow, SLOs.
- Governance: RBAC, secrets, policies, network isolation.

### 3) Azure service selection (reference)

- Device connectivity: Azure IoT Hub, Azure IoT Operations, IoT Edge.
- Event streaming: Event Hubs, Service Bus, Event Grid.
- Storage: Blob Storage, Data Lake, Cosmos DB, SQL.
- Analytics: Azure Data Explorer, Stream Analytics, Fabric/Synapse.
- APIs and applications: API Management, App Service, Container Apps, Functions.
- Monitoring: Azure Monitor, Application Insights, Log Analytics.
- Security: Key Vault, Defender for IoT, Private Endpoints, Managed Identity.

### 4) Non-functional design

Define and document:

- Reliability model (zones/regions, retries, dead-letter handling, replay).
- Security controls (zero trust, encryption, secret rotation, least privilege).
- Cost controls (retention tiers, rightsizing, autoscaling, workload scheduling).
- Data lifecycle (raw, curated, aggregated, archived).

### 5) Delivery plan

Create a phased execution:

- Phase 1: Pilot district or single use case.
- Phase 2: Multi-domain integration.
- Phase 3: City-scale rollout and optimization.

For each phase, include:

- Exit criteria
- Dependencies
- Risks and mitigations
- KPI set

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: azure-smart-city-iot-solution-builder
