# asian-sentry-techniques

Field notes on using AI as a co-composer — orchestration, composition, and the gap between "generate something" and "make something that means something."

This is a practitioner's notebook, not a tutorial. If you're looking for a polished guide, this isn't it. If you're working through the same questions — how do you think with these models rather than just prompt them — it might be useful.

---

## What this is

I work in Logic Pro. I've been using foundation models to think through composition problems: structure, orchestration decisions, harmonic motion, arrangement logic. Not as an autocomplete layer that fills bars — as a thinking partner that forces me to articulate what I actually want.

That distinction matters. Autocomplete gives you plausible next notes. A co-composer asks you what you're trying to do and pushes back when your answer is vague.

These notes document what I've learned from that process: what works, what doesn't, where the models are genuinely useful and where they're confidently wrong.

---

## Why "thinking in public"

The field is moving fast enough that polished tutorials are obsolete before they're finished. What's more durable is the working method — how to ask, how to evaluate the answer, when to trust it, when to override it.

So this is swyx-style thinking in public. Notes get updated when something changes. Dead ends stay in so you can see why they didn't work.

---

## Topics

### LLMs for composition structure and decision-making

Using language models to reason about musical form — not to generate notation, but to think through structural problems:

- Articulating the architecture of a piece before writing it
- Using model responses to stress-test ideas ("does this modulation make structural sense, or am I just avoiding commitment?")
- Generating decision trees for arrangement: what serves this section, what's distracting
- Working with the model as a sounding board when you'd otherwise just be stuck

The models are better at this than most people expect, because composition decisions are partly linguistic — you have to be able to describe what you want before you can make it.

### AI-assisted orchestration in Logic Pro

Practical notes on the workflow:

- Prompt techniques that produce useful orchestration suggestions vs. generic output
- How to describe a sonic texture so the model gives you something actionable
- Using model output as a starting constraint, not a final answer
- Where the model's knowledge of orchestration conventions is reliable vs. where it hallucinates confident nonsense
- Integration patterns: when to break out of the DAW and think in text, when to get back in and just play

Logic Pro specifics: channel strip decisions, MIDI orchestration, layering approaches, when software instruments are good enough and when they're not.

### Prompt techniques for musical ideas

The thing most people get wrong: asking for music. You don't want the model to generate music. You want it to help you think more clearly about music you're making.

Prompts that work:
- "I have these four bars. What structural problem are they setting up and what are my three most credible options for resolving it?"
- "Describe this texture as if you were writing liner notes for someone who can't hear it. What am I prioritising and what am I sacrificing?"
- "This section feels like it's trying to do two things. Identify them."

Prompts that produce noise:
- "Write me a chord progression for a melancholy piece"
- "What should come after this?"
- Anything where the model can give a plausible answer without understanding your actual intent

---

## What I'm currently working on

Notes on active experiments live in the repo as they accumulate. The README gets updated when the main lines of thinking shift.

---

## Philosophy

The underlying assumption here — shared with my writing work — is that AI tools are most useful when they're in the loop on your thinking process, not just your output process. Ask a model to do the thing, and you get a thing. Ask a model to help you think through the thing, and you get better at the thing.

That's the same philosophy behind [bullpen](https://github.com/cclawton/bullpen), which applies the same approach to writing: specialist agents that do one job, a human editor making every structural decision, no pretence that the model has taste.

The model doesn't have taste. It has pattern recognition at scale. The combination of that with someone who does have taste is genuinely interesting.

---

## See also

- [bullpen](https://github.com/cclawton/bullpen) — the writing equivalent: AI-assisted drafting pipeline with the same co-author philosophy applied to text
- [github.com/cclawton](https://github.com/cclawton) — other projects in the same space
