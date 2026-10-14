<!-- Generated supporting document. -->

# EvMem â€” Conceptual Architecture

<p align="center"><a href="https://evsphere.vercel.app/evmem"><img src="https://img.shields.io/badge/EvSphere-EvMem-0b0c0d?style=for-the-badge&logo=github&logoColor=white" alt="EvMem" /></a></p>

> **Scope note.** This describes what each subsystem is *for* and how responsibility is divided. It is not an implementation specification, and internal design detail is deliberately not published. Nothing here is sufficient to reconstruct the system.

---

## One-line model

A memory service that captures, retains, selects and retrieves â€” so relevant memories participate in computation while unrelated ones stay inactive.

---

## Subsystems

| Subsystem | Responsibility |
|---|---|
| **Capture** | Session events enter the system as they occur. |
| **Selection** | A filter decides which memories are relevant right now. |
| **Storage** | A persistent store retains raw information, not just summaries. |
| **Retrieval** | Relevant memory nodes are surfaced for the active task. |
| **Update** | What happened during a run is written back for future sessions. |
| **Decision Layer** | EvSystem-I bridges selection and the agent harness. |
| **Configuration** | Held separately from stored data, in its own file. |

---

## Design principles

1. **Explicit boundaries.** Each subsystem has one job. Overlap between them is a defect, not a convenience.
2. **Composition over configuration.** Capabilities are assembled at runtime rather than hard-wired at build time.
3. **Observability before optimisation.** A subsystem that cannot be inspected cannot be trusted or improved.
4. **Local first.** Execution and data stay under the operator's control wherever that is possible.
5. **Honest failure.** If something does not work, it says so rather than degrading silently.

---

## What is deliberately not here

- Source code, prompts, configuration or infrastructure
- Endpoint, credential, key or connection detail of any kind
- Dataset contents or identifiers
- Anything about a specific client or engagement
- Internal design rationale that would assist copying or attack

If you need any of the above, [ask directly](https://evsphere.vercel.app/start).

---

## Further reading

| | |
|---|---|
| [README](./README.md) | Overview |
| [docs/HOW-IT-WORKS.md](./docs/HOW-IT-WORKS.md) | Stage by stage |
| [docs/STATUS.md](./docs/STATUS.md) | Maturity and limits |
| [docs/FAQ.md](./docs/FAQ.md) | Questions and honest answers |

---

ðŸŒ [Website](https://evsphere.vercel.app) Â· [GitHub](https://github.com/evsphereofficial) Â· [npm](https://www.npmjs.com/~evsphere) Â· [LinkedIn](https://www.linkedin.com/company/evsphere) Â· [X](https://x.com/evsphereco)
