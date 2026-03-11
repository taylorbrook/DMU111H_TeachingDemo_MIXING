# Intro to Audio Mixing

---

## What is Mixing?

"We are mixing engineers, but more importantly: we are *sonic artists*."
— Roey Izhaki, *Mixing Audio*

Mixing is the process of combining individual recorded tracks into a finished stereo (or surround) piece. It is both a technical craft and a creative art form.

---

## Owsinski's Six Elements of a Mix

Bobby Owsinski's framework from *The Mixing Engineer's Handbook* organizes everything in a mix into six elements:

![The Six Elements of a Mix](diagrams/01-six-elements.svg)

---

## Signal Flow

![Signal Flow](diagrams/02-signal-flow.svg)

**Key concept**: Use **inserts** for processing that's unique to a channel (EQ, compression). Use **sends** for effects shared across multiple channels (reverb, delay). This creates a cohesive sense of space and saves CPU.

---

## EQ (Equalization)

EQ shapes the **frequency content** of a sound — what you hear as tone, brightness, warmth, or muddiness.

### The Frequency Spectrum

![The Frequency Spectrum](diagrams/03-frequency-spectrum.svg)

### Owsinski's Six Trouble Frequency Areas

| Frequency | Problem | Solution |
|-----------|---------|----------|
| ~200 Hz | Mud, boominess | HPF or gentle cut |
| 300-500 Hz | Boxiness | Narrow cut |
| ~800 Hz | Cheap, hollow | Narrow cut |
| 1-1.5 kHz | Nasal, honky | Narrow cut |
| 4-6 kHz | Harsh, sibilant | Gentle cut or de-esser |
| 10 kHz+ | Hiss, sibilance | Shelf cut or de-esser |

### Best Practices of EQ

- **Subtractive first**: Cut problem frequencies before boosting desired ones — introduces fewer artifacts (Senior, *Mixing Secrets*)
- **HPF on everything**: Unless it's bass or kick, high-pass filter to remove unnecessary low-end rumble.
- **Cut narrow, boost wide**: Surgical cuts target problems; broad boosts sound more natural
- **Don't use it if it doesn't need it!

---

## Compression

Compression controls **dynamic range** — the difference between the loudest and quietest parts of a signal.

### How It Works

![How Compression Works](diagrams/04-compression.svg)

### The Compression Curve

![The Compression Curve](diagrams/04b-compression-curve.svg)

### Key Parameters

| Parameter | What It Does | Think of It As... |
|-----------|-------------|-------------------|
| **Threshold** | Level where compression begins | The "trigger point" |
| **Ratio** | How much to reduce above threshold | How aggressively the dynamic range is compressed |
| **Attack** | How quickly compression engages | Fast = catches transients; Slow = lets transients through |
| **Release** | How quickly compression stops | Fast = can produce a pumping effect; Slow = smooth |
| **Makeup Gain** | Boosts output to compensate for reduction | Restoring perceived volume |

### Best Practices

- **Start gentle**: Low ratio (2:1-4:1), moderate threshold, and adjust from there
- **Listen, don't just look at meters**: Use your ears, not the gain reduction display
- **Compression is a balance tool**: "From a mix perspective, the primary purpose of compression is to achieve a stable balance." — Mike Senior, *Mixing Secrets*
- **The fader instability diagnostic**: If you keep adjusting a fader, that track probably needs compression (Senior)

---

## Reverb

Reverb can create a gobal sense of **space** and can also be used as an effect on a single track or subgroup.

Today we will focus on the idea of a global reverb that helps to create a sense of shared space and coherence to a mix.

### The Sound Stage (after Huber & Moylan)

![The Sound Stage](diagrams/05-sound-stage.svg)

### Key Parameters

| Parameter | What It Does | Tip |
|-----------|-------------|-----|
| **Pre-delay** | Gap before reverb begins | Longer = keeps lead element clear and upfront |
| **Decay time** | Length of reverb tail | Consider matching to song tempo — reverb can be rhythmic |
| **Wet/dry** | Blend of effect vs. original | Less is usually more |
| **Type** | Hall, room, plate, spring, etc. | Each has a character; experiment and get to know the sound of these different types|

### Best Practices

- **Use sends, not inserts for additive effects like reverb**: Route multiple channels to a shared reverb bus with 100% wet and 0% dry signal to control how much reverb is added to the mix and cohere various parts together into the same virtual space

---

## Panning

![Panning — Stereo Placement](diagrams/06-panning.svg)

Some typical panning:
- **Centre**: Lead, bass, primary rhythm
- **Sides**: Harmony, secondary elements, texture, percussion
- **Check in mono**: If panned elements disappear in mono, there may be phase issues

---

## Mixing Workflow Summary

![Mixing Workflow](diagrams/07-mixing-workflow.svg?v=2)

---

## Free Resources

| Resource | What It Is | URL |
|----------|-----------|-----|
| **cambridge-mt.com** | 500+ free multitrack sessions for mixing practice | cambridge-mt.com/ms/mtk/ |
| **iZotope Learn Hub** | Free articles and guides on mixing fundamentals | izotope.com/en/learn |
| **Produce Like A Pro (YouTube)** | Full mixing tutorials with free multitracks | YouTube |

## Recommended Reading

- **Bobby Owsinski** — *The Mixing Engineer's Handbook* (5th ed., 2022) — Accessible framework + engineer interviews
- **Mike Senior** — *Mixing Secrets for the Small Studio* (2nd ed., 2019) — Practical, budget-friendly, hands-on
- **Roey Izhaki** — *Mixing Audio* (4th ed., 2024) — Comprehensive technical reference
- **William Moylan** — *The Art of Recording* (2002/2015) — Deep analytical and aesthetic perspective
- **David Miles Huber** — *Modern Recording Techniques* (9th ed., 2017) — Broad survey of the full recording chain
