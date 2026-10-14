<!-- Generated supporting document. -->

# EvMem â€” How It Works

[â† Back to README](./README.md)

---

- Captures session events as they happen rather than summarising at the end
- Selects which memories are relevant to the current task
- Retains raw information instead of immediately compressing it into semantics
- Retrieves memory nodes in a context-dependent way
- Updates memory as runs complete, so later sessions benefit
- Serves locally with its own configuration boundary

---

## Stage by stage

| # | Stage | What happens |
|---|---|---|
| **1. Session** | An agent run begins and produces events. |
| **2. Capture** | Events are recorded rather than discarded at session end. |
| **3. Select** | A filter determines what is relevant to the current task. |
| **4. Retrieve** | Relevant memory nodes are activated. |
| **5. Reason** | The agent works with only the activated memory. |
| **6. Update** | The outcome is written back, extending the store. |

---

## Where the boundaries are

Each stage above hands something to the next one. Those hand-offs are the interesting part: they are where correctness is decided, and they are the first place to look when something misbehaves.

What is deliberately not documented: internal data structures, specific algorithms, thresholds, or the contents of any configuration. That is not an oversight â€” publishing them would make the system easier to copy or interfere with.

---

## Verifying behaviour yourself

The only honest way to judge EvMem is to run it and observe. Claims in this repository are consistent with what the published artefacts show, but the artefacts are captures and schematics, not proofs.

- Maturity: **In development**
- Reference: [https://evsphere.vercel.app/evmem](https://evsphere.vercel.app/evmem)

---

ðŸŒ [Website](https://evsphere.vercel.app) Â· [GitHub](https://github.com/evsphereofficial) Â· [npm](https://www.npmjs.com/~evsphere) Â· [LinkedIn](https://www.linkedin.com/company/evsphere) Â· [X](https://x.com/evsphereco)
