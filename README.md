# Whaber Oracle Agent Card

Ground truth operational layer for urban transfers in Latin America.

## Live Endpoint

https://oracle.whaber.ai/.well-known/agent-card.json

## What is Whaber Oracle?

Whaber Oracle is the Layer 4 execution infrastructure for travel AI in LatAm — the layer between a booking and a verified ground transfer.

Any A2A-compatible agent can discover and consume the Oracle via the canonical endpoint above.

## 5 Core Tools — Agent Kit v1 (Partner-Only)

| Tool | Description |
|------|-------------|
| whaber_get_safe_pickup_point | Physically verified pickup point for a hotel or airport in Quito |
| whaber_calculate_ops_window | Operational time window with Quito traffic buffers and ANT compliance |
| whaber_validate_carrier_compliance | ANT operating permit validation for Ecuador carriers |
| whaber_query_place_safety | Zone safety classification (safe / caution / avoid) for a time window |
| whaber_get_hotel_context | Operational context for hotels registered in the Place Graph |

## Place Graph

- 17 zones with full operational cataloging — Quito, Ecuador
- Latency p95: less than 50ms
- Safety scores recomputed automatically via driver field reports
- Numeric scores never exposed — semantic labels only

## Security and Compliance

- Authentication: Bearer token required
- HTTPS: TLS via Cloudflare
- Ecuador LOPDP compliant
- ANT carrier verification
- 6-gate validation pipeline
- Full audit trail via EventStore

## Active Pilot

NH Collection Quito.
Partner-Only soft launch Q2 2026.

---

Whaber Travel-Ops · oracle@whaber.ai · https://whaber.ai
