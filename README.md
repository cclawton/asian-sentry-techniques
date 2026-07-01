# asian-sentry-techniques

AI-driven music composition project — a 5-song EP built around the classical elements (Wood, Water, Metal, Fire, Earth), co-driven with AI agents in Logic Pro. Each song evokes its element through lyrics, sounds, tone, and composition. Field notes on using LLMs for MIDI generation, sound design, mixing, and automation across the full production pipeline.

---

## The project

Asian Sentry is a 5-song EP where each element is a complete song with its own sonic identity:

| Element | Lyrical theme | Sonic palette | Compositional tone |
|---------|---------------|---------------|-------------------|
| Wood | Growth, roots, reaching | Organic, woody, resonant | Warm, unfolding |
| Water | Flow, reflection, erosion | Glassy, fluid, sustained | Slow, evolving |
| Metal | Edge, precision, resonance | Sharp, metallic, bell-like | Sharp, rhythmic |
| Fire | Consumption, transformation, light | Bright, distorted, dynamic | Intense, building |
| Earth | Ground, weight, patience | Deep, grounded, granular | Patient, heavy |

Every song starts with an existing idea — audio, MIDI, or lyrics. The AI's job is to develop that seed into a finished demo, not to generate the seed.

---

## How AI is in the loop

The approach is co-driving, not delegating. AI agents help with:

- **Composition development** — take an existing riff, progression, or lyric and help think through structure, harmonic direction, and arrangement logic
- **MIDI generation** — complementary basslines, counter-melodies, arpeggios, rhythmic patterns generated as Python scripts that produce MIDI files for Logic Pro
- **Sound design** — instrument and layering suggestions that serve each element's sonic palette
- **Lyrics** — verse/chorus/bridge development that extends the elemental theme without repeating it
- **Mixing guidance** — EQ moves, compression decisions, spatial placement, frequency problem diagnosis
- **Automation** — volume, filter, and parameter movement plans for build/release architecture
- **EP-level review** — how the five songs work as a sequence, track order, contrast and continuity

---

## The workflow

1. **Bring a seed** — an existing audio riff, MIDI progression, or lyric phrase
2. **Develop structure** — what form serves this element? Where does tension build and release?
3. **Generate complementary MIDI** — basslines, counter-melodies, arpeggios via Python + MIDI libraries
4. **Sound design** — instrument categories and layering that evoke the element
5. **Lyrics and vocal direction** — thematic development, syllable-matched verses, chorus writing
6. **Mixing and automation** — per-track EQ, dynamics, spatial, and automation maps
7. **EP-level review** — sequence, contrast, gaps across all five pieces

---

## What works and what doesn't

**Works well:**
- Structural and harmonic reasoning (the LLM understands music theory deeply)
- Developing an existing seed into something larger
- Sound selection as category-level guidance
- Mix diagnosis from plain-language descriptions
- Generating MIDI via Python scripts (precise, repeatable, editable)
- Lyric collaboration when you provide the theme and constraints

**Doesn't work:**
- Asking the model to "write a song" — you get generic output with no taste
- Generating music with no seed or direction
- Specific plugin/preset recommendations — the model doesn't know your rig
- Generating audio directly — MIDI + sound selection is the right abstraction layer
- Anything where you accept the first answer without filtering through your own taste

---

## Tools in the stack

- **Logic Pro** — DAW, software instruments, mixing
- **LLMs (Claude)** — composition thinking, MIDI generation, sound design, mixing guidance, lyrics
- **Python + MIDI libraries** (`mido`, `pretty_midi`) — programmatic MIDI construction
- **AudioCipher** — MIDI idea generation library (seed material)
- This repo — field notes, techniques, and code as they develop

---

## Philosophy

The model doesn't have taste. It has pattern recognition at scale. The combination of that with someone who does have taste is genuinely interesting.

Every song starts with a human idea. The AI develops it, pressures it, suggests directions, generates complementary material, and helps with the technical pipeline. But the seed and the final call are always human.

Same philosophy as [bullpen](https://github.com/cclawton/bullpen) — AI-assisted creative work where the human makes every structural decision and the model does the heavy lifting on execution. Different domain, same principle.

---

## See also

- [bullpen](https://github.com/cclawton/bullpen) — the writing equivalent: AI-assisted drafting pipeline with the same co-author philosophy applied to text
- [github.com/cclawton](https://github.com/cclawton) — other projects in the same space
