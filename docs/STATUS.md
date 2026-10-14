<!-- Generated supporting document. -->

# EvMem â€” Status and Limits

[â† Back to README](./README.md)

---

## Current state

| | |
|---|---|
| **Maturity** | **In development** |
| **Version** | bundled with 0.7.3 |
| **Public page** | [https://evsphere.vercel.app/evmem](https://evsphere.vercel.app/evmem) |
| **Machine-readable** | [llms.txt](https://evsphere.vercel.app/llms.txt) |

---

## What the maturity label means

| Label | Meaning |
|---|---|
| **Active** | An operating service or activity, running now. |
| **Available** | Usable by someone outside the team, under the stated conditions. |
| **Experimental** | A research prototype. Results are reported, not settled. |
| **In development** | Actively built. Capabilities can change without notice. |
| **Planned** | Intended direction, not implemented. |

EvMem is currently **In development**.

---

## Known limits

- Not distributed independently â€” currently reachable only through the EvAgent package
- Closed source; no standalone package or public repository
- Its configuration file holds an API key and a model base URL and must never be committed or captured
- Setup downloads an embedding model of roughly 634 MB
- No public schema documentation; any diagram published is sanitised
- No security or privacy certification is claimed

---

## What you need to run it

- EvAgent installed â€” EvMem ships inside @evsphere/evagent
- An embedding provider
- Local disk for stored memory and the embedding model

---

## What is *not* claimed

- No accuracy, reliability or safety guarantee
- No user count, adoption figure or performance benchmark
- No endorsement, certification or independent review
- No timeline and no promise of a future release

EvMem is not claimed to be finished, production-ready or commercially supported.

---

ðŸŒ [Website](https://evsphere.vercel.app) Â· [GitHub](https://github.com/evsphereofficial) Â· [npm](https://www.npmjs.com/~evsphere) Â· [LinkedIn](https://www.linkedin.com/company/evsphere) Â· [X](https://x.com/evsphereco)
