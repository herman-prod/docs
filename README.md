# AARM — Autonomous Action Runtime Management

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Docs](https://img.shields.io/badge/docs-aarm.dev-blue)](https://aarm.dev)

**An open system specification for securing AI-driven actions at runtime.**

---

## What is AARM?

As AI systems evolve from text generators into autonomous agents executing consequential actions—API calls, database mutations, financial transactions—the security boundary shifts from model outputs to **tool execution**.

AARM defines what a runtime security system must do:

1. **Intercept** actions before execution
2. **Evaluate** against policy
3. **Enforce** decisions (allow / deny / modify / require approval)
4. **Record** tamper-evident receipts
```
Agent ──► AARM System ──► Tools/APIs
              │
              ▼
        Action Receipts
```

---

## Why AARM?

Traditional security doesn't address AI-driven actions:

- **SIEM** — observes *after* execution; can't prevent harm
- **API gateways** — verify *who*, not *what* the action means
- **Firewalls** — agents operate *inside* the perimeter
- **Prompt guardrails** — filter text, not actions
- **Human-in-the-loop** — doesn't scale; can be exploited

AARM fills this gap with runtime enforcement at the action layer.

---

## Documentation

**[aarm.dev](https://aarm.dev)**

---

## Quick Links

| Resource | Description |
|----------|-------------|
| [Specification](https://aarm.dev/) | Problem, definition, components |
| [Threat Model](https://aarm.dev/threats/overview) | What AARM defends against |
| [Architectures](https://aarm.dev/architectures/overview) | Gateway, SDK, eBPF options |
| [Conformance](https://aarm.dev/conformance/requirements) | R1–R8 requirements |
| [Research Paper](https://aarm.dev/research/technical-paper) | IEEE-style technical paper |

---

## Contributing

Contributions welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Local Development
```bash
npm i -g mint    # Install Mintlify CLI
mint dev         # Run at http://localhost:3000
```

---

## License

[MIT](LICENSE)

---

<p align="center"><em>SIEM was built for events. AARM is built for actions.</em></p>
