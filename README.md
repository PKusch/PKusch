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

| | What it does | Why it matters |
|---|---|---|
| **[sequela](https://github.com/PKusch/sequela)** | Tests whether an AI agent can say what its own next action will do, and then acts on what it said. | The right answer is worked out from the tool itself, so there is no judge to argue with. 251 test calls; no live model has been run yet, and the README says so first. |
| **[airlock](https://github.com/PKusch/airlock)** | Shows a person, in plain words, what an agent's tool call will do before it runs. | The words are built from the facts of the call, not written by the agent, so the agent cannot talk anyone into approving it. Tested against 36 real tools nobody here wrote, which found four defects the home-made tests never could. Attacking its own proxy later found calls that got through unjudged when batched or malformed; those are fixed, and the README says so. |
| **[remit](https://github.com/PKusch/remit)** | A rulebook for what an AI agent may do without asking a person, mapped to the EU AI Act, NIST AI RMF, ISO 42001 and DORA. | Two engineers looking at the same failure write it up the same way: four independent assessors agreed at 0.83, where 0.61 counts as good. |
| **[tendere-ai](https://github.com/PKusch/tendere-ai)** | Matches consultants to work by what they can do, how recently, and what proves it, instead of one score. | It can tell *never done it* from *did it years ago* from *can do it but cannot prove it*, and shows leaders which scarce skills people have but cannot yet prove. Built for a hackathon on made-up data, and the README says so. |
| **[eightball](https://github.com/PKusch/eightball)** | A Magic 8 Ball that answers from a small AI model on your own machine, and only ever with the 20 classic phrases. | It reads the model's odds rather than its words, so it can hand back "reply hazy" when it is not sure — safer, not smarter: it speaks far less often and is wrong far less often when it does. |
| **[terroir-study](https://github.com/PKusch/terroir-study)** | A map for studying wine, for the WSET Level 3 exam: France, Italy, Spain, Germany and the New World. | Click a region, zoom in to its villages, follow the chain from climate to what is in the glass, then get quizzed on the *why*. 165 questions that remember what you got wrong, and a tasting drill marked against the grape. |
| **[berghain-bouncer](https://github.com/PKusch/berghain-bouncer)** | A voice doorman for a Berlin techno club that turns almost everyone away. | Built in under an hour at a meetup. The verdict is stamped on screen, so the agent acts rather than just talks. |
