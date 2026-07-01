# asian-sentry-techniques

AI-driven music composition project — co-driving original music with AI agents in Logic Pro. Field notes on using LLMs for MIDI generation, sound design, mixing decisions, and automation. Not "AI makes a song" — a human composer using AI as a real-time collaborator across the entire production pipeline.

---

## What this is

Asian Sentry is an original music project working across five elemental themes — Wood, Water, Metal, Fire, Earth. Each element is a Logic Pro project with its own sonic identity. The question this repo explores: how do you use LLMs and AI tools to drive composition, orchestration, and mixing decisions when you're the one with taste?

The approach is co-driving, not delegating. AI agents help with:

- **MIDI generation** — chord progressions, melodies, basslines, rhythmic patterns, counterpoint
- **Sound selection** — which instrument/preset serves the emotional intent of a section
- **Mixing guidance** — EQ decisions, spatial placement, dynamics, reference targets
- **Automation** — parameter movement over time, build/release architecture
- **Structural decisions** — arrangement logic, section transitions, tension/release maps
- **Harmonic analysis** — what's actually happening in a progression, where it could go next

---

## The workflow

### 1. Composition thinking (LLM as sounding board)

Before touching MIDI, use the LLM to think through the architecture:

- "I'm writing a piece for the Water element. Slow, fluid, glassy. What structural arch supports that without becoming ambient wallpaper?"
- "I have these four bars. What are my three most credible options for where this goes next?"
- "This section feels like it's trying to do two things. Identify them."

The model is better at this than most people expect because composition decisions are partly linguistic — you have to describe what you want before you can make it.

### 2. MIDI generation (LLM + MIDI tools)

Use the LLM to generate MIDI-compatible musical ideas:

- **Chord progressions** — describe the emotional arc, get progressions in a specific key/mode
- **Melodies** — give context (chords, mood, tempo), get melodic options as note data
- **Basslines and counterpoint** — harmonic support that serves without cluttering
- **Rhythmic patterns** — groove suggestions for specific genres/feels

MIDI can be exported directly into Logic Pro. The LLM can also generate Python scripts that programmatically construct MIDI files for more complex patterns.

### 3. Sound design (LLM as orchestrator)

- Describe the sonic texture you're after → get instrument, preset, and layering suggestions
- "I need something that sits between a pad and a bell — present but not sharp, sustaining but not ambient"
- The model knows orchestration conventions well enough to suggest layering (strings + synth pad, clean guitar + reverse reverb, etc.)
- Where it's less reliable: specific plugin/preset names — treat those as categories, not exact recommendations

### 4. Mixing (LLM as mix engineer)

- Describe your mix problem in plain language → get actionable EQ, compression, and spatial suggestions
- "The low-mids are muddy in the Water piece — what's likely causing it and what are my moves?"
- Reference track analysis: describe a commercial mix you admire → get a breakdown of likely techniques
- Automation maps: "Give me a volume and filter automation plan for a 4-minute build"

### 5. Structural review (LLM as producer)

- Export your arrangement as a text description (section names, bars, instrumentation) → get structural feedback
- "Here's my arrangement: Intro(8) - Verse(16) - Pre(8) - Chorus(16) - Break(8) - Chorus(16) - Outro(8). Where does energy dip?"
- The model catches things you miss when you've been listening on loop for three hours

---

## What works and what doesn't

**Works well:**
- Structural and harmonic reasoning (the LLM understands music theory deeply)
- Sound selection as category-level guidance
- Mix diagnosis from plain-language descriptions
- Generating MIDI via Python scripts (precise, repeatable, editable)

**Doesn't work:**
- Asking the model to "write a song" — you get generic output with no taste
- Specific plugin/preset recommendations — the model doesn't know your rig
- Generating audio directly — MIDI + sound selection is the right abstraction layer
- Anything where you accept the first answer without filtering through your own taste

---

## Tools in the stack

- **Logic Pro** — DAW, software instruments, mixing
- **LLMs (Claude)** — composition thinking, MIDI generation, sound design, mixing guidance
- **Python + MIDI libraries** (`mido`, `pretty_midi`) — programmatic MIDI construction
- **AudioCipher** — MIDI idea generation library (serves as seed material)
- This repo — field notes, techniques, and code as they develop

---

## Philosophy

The model doesn't have taste. It has pattern recognition at scale. The combination of that with someone who does have taste is genuinely interesting.

Same philosophy as [bullpen](https://github.com/cclawton/bullpen) — AI-assisted creative work where the human makes every structural decision and the model does the heavy lifting on execution. Different domain, same principle.

---

## See also

- [bullpen](https://github.com/cclawton/bullpen) — the writing equivalent: AI-assisted drafting pipeline with the same co-author philosophy applied to text
- [github.com/cclawton](https://github.com/cclawton) — other projects in the same space
