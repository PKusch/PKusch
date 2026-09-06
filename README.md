**I build the parts of an agent system that decide what the agent is allowed to do — and I publish the measurements, including the ones that went against me.**

Most of what is here is governance and consent infrastructure for AI agents: what an
agent may do without asking anyone, how the person it does ask is protected from being
lied to, and how to write down what went wrong afterwards so that two engineers looking
at the same incident record the same thing. I came to it from a career delivering change
inside banks, which is where I learned that the failures worth worrying about are the
quiet ones.

Everything here is public, MIT unless the repo says otherwise, and runs from a clean clone.

---

### Selected work

| | What it is | Why it might interest you |
|---|---|---|
| **[airlock](https://github.com/PKusch/airlock)** | Consent for agent tool calls | A consent prompt that asks a model to *describe* a pending tool call lets the arguments write the sentence a person approves. Airlock derives the consequence in code, lets the model only frame it, and rejects any framing that understates what was derived. Tested against a fully compromised narrator, then against 36 MCP tool definitions nobody here wrote — which found four defects the hand-written fixtures never could. |
| **[remit](https://github.com/PKusch/remit)** | Agentic skills framework for AI governance | Existing frameworks ask whether a model is fair. None ask how large a single action's blast radius is, or whether the human in the loop could realistically say no. Autonomy tiers and a diagnostic manual for agent failure modes, over EU AI Act, NIST AI RMF, ISO 42001 and DORA. A blind panel of four assessors reached Fleiss' κ = 0.83 on the manual. |
| **[tendere-ai](https://github.com/PKusch/tendere-ai)** | Consulting bench engine that maps people instead of ranking them | Every capability carries level, recency and evidence, never one number, so it can tell *never done it* from *did it but it has gone cold* from *can do it but cannot prove it*. Built for a hackathon; the data is synthetic and the README says so. |
| **[terroir-study](https://github.com/PKusch/terroir-study)** | Map-first study tool for WSET Level 3 | Wine knowledge is spatial, and every study app treats it as trivia. Click a region, follow the chain from climate to glass, then get quizzed on the *why*. Hand-projected SVG map, no UI libraries. |
| **[berghain-bouncer](https://github.com/PKusch/berghain-bouncer)** | A voice-agent doorman that turns almost everyone away | Built in under an hour at a voice AI meetup. One WebSocket does speech, reasoning and speech back; the verdict is a tool call rendered as a stamp on screen, so the agent acts rather than just talks. |

---

### Background

Management consulting: AI, product and financial-services transformation. Large-scale
change in regulated environments — business analysis, product delivery, agile ways of
working, operating-model modernisation across enterprise programmes. Regulatory literacy
(DORA, EU AI Act, NIST AI RMF, ISO 42001) is why the governance work above is grounded
rather than theoretical.
