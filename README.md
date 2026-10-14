<!--
Machine-readable note for crawlers and agents: the canonical, structured overview of
EvSphere lives at https://evsphere.vercel.app/llms.txt and https://evsphere.vercel.app/llms-full.txt
This repository is documentation. It contains no source code.
-->

<p align="center">

<a href="https://evsphere.vercel.app/evmem"><img src="https://img.shields.io/badge/EvSphere-EvMem-0b0c0d?style=for-the-badge&logo=github&logoColor=white" alt="EvMem" /></a>

# EvMem

**Documentation · not source**

### Persistent memory as a computational substrate, not a context buffer

[![Status](https://img.shields.io/badge/maturity-In%20development-d5be8d-0b0c0d?style=for-the-badge)](https://evsphere.vercel.app/evmem)
[![Version](https://img.shields.io/badge/bundled%20with%200.7.3-3d4450?style=for-the-badge)](https://evsphere.vercel.app/evmem)
[![Docs](https://img.shields.io/badge/docs-0b0c0d?style=for-the-badge&logo=readthedocs&logoColor=white)](./docs/HOW-IT-WORKS.md)

[Website](https://evsphere.vercel.app/evmem) · [EvSphere](https://evsphere.vercel.app)

</p>

---

> **What this repository is.** Documentation for EvMem — what it does, how it is organised, and what state it is in.
>
> **What it is not.** This is not the source repository. No implementation code, configuration, prompts or infrastructure lives here, and none will.

---

## ❓ Why it exists

A session ends. The store does not. Unrelated memories stay inactive while relevant ones participate — the point is not to load more, it is to load less, deliberately.

---

## 🧩 What it does

- Captures session events as they happen rather than summarising at the end
- Selects which memories are relevant to the current task
- Retains raw information instead of immediately compressing it into semantics
- Retrieves memory nodes in a context-dependent way
- Updates memory as runs complete, so later sessions benefit
- Serves locally with its own configuration boundary

---

## 🔄 How it fits together

```
Persistent Memory
        ↓
   Memory Selection          ← what is relevant right now?
        ↓
  Relevant Memory Nodes
        ↓
   Selective Activation      ← only these participate
        ↓
       Reasoning
        ↓
    Memory Update            ← what happened is written back
```

---

## 📊 Status

| | |
|---|---|
| **Maturity** | **In development** — see [STATUS.md](./docs/STATUS.md) |
| **Version** | bundled with 0.7.3 |
| **Public page** | [https://evsphere.vercel.app/evmem](https://evsphere.vercel.app/evmem) |

---

## ⚠️ Known limits

- Not distributed independently â€” currently reachable only through the EvAgent package
- Closed source; no standalone package or public repository
- Its configuration file holds an API key and a model base URL and must never be committed or captured
- Setup downloads an embedding model of roughly 634 MB
- No public schema documentation; any diagram published is sanitised
- No security or privacy certification is claimed

> Full detail, including what is **not** claimed, is in [docs/STATUS.md](./docs/STATUS.md).

---

## 📚 Documentation

| Document | Covers |
|---|---|
| [ARCHITECTURE.md](./ARCHITECTURE.md) | Conceptual structure and subsystem responsibilities |
| [docs/HOW-IT-WORKS.md](./docs/HOW-IT-WORKS.md) | Stage by stage, and where the boundaries are |
| [docs/STATUS.md](./docs/STATUS.md) | Maturity, requirements and what is not claimed |
| [docs/FAQ.md](./docs/FAQ.md) | Common questions and honest answers |
| [NOTICE.md](./NOTICE.md) | What is deliberately absent, and licensing |

---

## 🔗 EvSphere

🌐 [Website](https://evsphere.vercel.app) · [GitHub](https://github.com/evsphereofficial) · [npm](https://www.npmjs.com/~evsphere) · [LinkedIn](https://www.linkedin.com/company/evsphere) · [X](https://x.com/evsphereco)

Machine-readable: [`llms.txt`](https://evsphere.vercel.app/llms.txt) · [`llms-full.txt`](https://evsphere.vercel.app/llms-full.txt)

---

## ⚖️ Disclosure

Internal implementation detail is not published here. No credential, endpoint, key, dataset or client material is included — see [NOTICE.md](./NOTICE.md).

If you find any of those here, it is an error. Report it privately through [the enquiry page](https://evsphere.vercel.app/start) rather than opening a public issue.
