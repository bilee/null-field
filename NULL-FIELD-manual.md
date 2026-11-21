# NULL·FIELD — User Manual

*A generative dark-matter synthesizer you play with glowing dots and floating orbs.*

NULL·FIELD runs entirely in your web browser. It combines a drifting drone pad, an arpeggiator, bouncing "orb" glitch sounds, a classic drum machine, a Euclidean polyrhythm machine and an Amen-style break chopper — all of which can evolve on their own while you play.

---

## Contents

1. [Getting started](#1-getting-started)
2. [Screen overview](#2-screen-overview)
3. [The top bar](#3-the-top-bar)
4. [The field: dots and orbs](#4-the-field-dots-and-orbs)
5. [The drum strip](#5-the-drum-strip)
6. [The dock: tabs and knobs](#6-the-dock-tabs-and-knobs)
7. [Harmony](#7-harmony)
8. [Arp (arpeggiator)](#8-arp-arpeggiator)
9. [Pad (drone + 2 LFOs)](#9-pad-drone--2-lfos)
10. [Drums](#10-drums)
11. [Euclid (glitch percussion)](#11-euclid-glitch-percussion)
12. [Break (break chopper)](#12-break-break-chopper)
13. [Orbs](#13-orbs)
14. [Glitch](#14-glitch)
15. [Master FX](#15-master-fx)
16. [Presets and sharing](#16-presets-and-sharing)
17. [Keyboard shortcuts](#17-keyboard-shortcuts)
18. [Tips and recipes](#18-tips-and-recipes)
19. [Troubleshooting](#19-troubleshooting)

---

## 1. Getting started

1. Open NULL·FIELD. The field is already moving, but it is silent.
2. Click **ENTER THE FIELD** (or press **Space**). Sound starts — browsers only allow audio after a click.
3. A chord is already held, the arpeggiator is playing, the pad is droning, and the drums roll a fresh random beat.
4. Click dots to change the notes, drag on empty space to throw orbs, and explore the tabs in the dock at the bottom.

> **Headphones are recommended.** Much of the sound lives in the sub-bass and stereo field.

---

## 2. Screen overview

| Area | Where | What it does |
|---|---|---|
| **Top bar** | Top edge | Start/stop, tempo, master volume, preset slots, sharing, randomize-all |
| **Readout** | Under the top bar | Current chord, clock, and a summary of the field |
| **Field** | Center | The grid of dots (notes) and floating orbs |
| **Drum strip** | Under the field | 6 × 16 squares — the drum machine pattern |
| **Dock** | Bottom edge | Tabbed controls for every module |

### The readout

- **chord** — the notes currently held (e.g. `E2 F3 B3 D4`).
- **clock** — bar and beat, tempo, and a countdown to the next automatic chord change (`next chord in 12 bars`). Shows `frozen · 0 bpm` when tempo is 0.
- **field** — arp pattern/rate/octaves, number of orbs, key and scale.
- The grey line below is a reminder of the main gestures.

---

## 3. The top bar

| Control | How to use it |
|---|---|
| **▶ START / ■ STOP** | Starts or stops all sequencing. Stopping releases the pad gently. |
| **TEMPO** knob | 0–255 BPM. At **0** the clock *freezes*: sequencers stop, but the pad keeps droning and orbs keep sounding when they hit notes. |
| **MASTER** knob | Overall output volume. |
| **PRESETS 1–8** | Click a slot to load it. Filled slots are outlined; the active slot is solid white. Right-click a slot to clear it. |
| **SAVE** | Press, then click a slot to store the current setup there (the slot outlines turn red while waiting). |
| **SHARE** | Opens a small panel to copy the current setup as a text code, or paste a code to load it. |
| **⚄ MUTATE ALL** | Randomizes almost everything (same as the **R** key). Save first if you like what you have! |

---

## 4. The field: dots and orbs

### Dots = notes

The field is a 12 × 8 grid of dots. Every dot is a note in the current key and scale:

- **Lower = lower pitch.** The bottom-left dot is the lowest note.
- Moving **one dot right** goes up one note of the scale.
- Moving **one row up** jumps up three scale notes (two for 5-note scales). The same note can therefore appear in several places, like on a guitar neck.
- Dots with a **small ring** are root notes of the key — use them to orient yourself.

**Click a dot** to hold that note; click it again to release it. Up to 8 notes can be held (adding a 9th drops the oldest). Held notes:

- feed the **arpeggiator**, which plays through them and draws glowing lines between them;
- feed the **pad**, which drones on them;
- become **bumpers** that orbs bounce off.

When you hold a dot while the music is playing, it plays a short note so you can hear what you chose.

### Orbs = glitch sounds

Orbs are glowing spheres that drift around the field.

| Gesture | Result |
|---|---|
| **Drag on empty space** and release | Throws an orb from where you started, in the direction you dragged. A longer drag throws faster. |
| **Click (tap) on empty space** | Drops an orb moving in a random direction. |
| **Right-click an orb** | Pops it. |

How orbs make sound:

- **Hitting a held dot** plays a glitch sound at that note's pitch (the sound is set in the **Orbs** tab).
- **Hitting another orb** plays a bell-like ping.
- **Hitting a wall** can make a low thud.
- Each **arp note pushes nearby orbs away** in a shockwave — so the arpeggiator and the orbs constantly stir each other up.

An orb's **color shows its sound voice**. Up to 24 orbs can exist; automatically spawned orbs fade out after a while, orbs you throw stay until you pop or clear them.

### Visual feedback

- Background clouds swell and sway with the **pad** and its **LFOs**.
- The whole field pulses on kick drums.
- Colored squares and streaks flash when the **Euclid** machine plays.
- Horizontal "screen tears" are glitch events.

---

## 5. The drum strip

Below the field are six rows of 16 squares — one bar of 16th notes for the main drum machine.

| Row | Drum |
|---|---|
| **KCK** | Kick |
| **SNR** | Snare |
| **CLP** | Clap |
| **RIM** | Rimshot |
| **CHH** | Closed hi-hat |
| **OHH** | Open hi-hat |

- **Click a square** to cycle it: *off → on → accent (brighter, louder) → off*.
- **Click a drum's name** to select it for editing in the **Drums** tab (the selected name turns amber).
- The highlighted column is the playhead. Every 4th square has a brighter outline to mark the beats.

---

## 6. The dock: tabs and knobs

The dock shows **one module at a time**. Each tab has its own color, and the dock background tints to match so you always know where you are.

**Tabs:** HARMONY · ARP · PAD · DRUMS · EUCLID · BREAK · ORBS · GLITCH · MASTER FX

A small **dot on a tab** (Arp, Drums, Euclid, Break) glows when that module is switched on.

### Dock tools (top right)

| Button | What it does |
|---|---|
| **preview off / on** | When on, sound-design knobs (Orbs, Euclid) play a short test hit as you turn them, and picking a drum or Euclid voice auditions it. Off by default. |
| **more ▸ / more ▾** | Shows or hides the deep settings. Extra groups appear with a **dashed border** and the label *· more*. The setting applies to all tabs. |
| **▾ hide / ▴ show** | Collapses the dock so the field fills the screen. |

The dock remembers your last tab and whether *more* was open.

### Using the knobs

| Action | Result |
|---|---|
| **Drag up / down** (or sideways) | Change the value |
| **Shift + drag** | Fine adjustment |
| **Double-click** | Reset to its starting value |
| **Mouse wheel** | Step up or down |
| **Arrow keys** (after clicking a knob) | Step up or down |

The value is shown under each knob. **Bipolar** knobs (tune, pan, sweep, pitch) start from the center.

Dropdowns pick from a list; **ON/OFF** buttons toggle a feature.

---

## 7. Harmony

*Color: violet.* Controls the key, the scale and how the chords evolve.

### Key

| Control | Description |
|---|---|
| **root** | The key's root note (C–B). |
| **scale** | phrygian, locrian, harmonic minor, phrygian dominant, double harmonic, hirajoshi, iwato, in sen — all chosen for a dark character. Changing it re-maps every dot instantly. |

### Motion

| Control | Description |
|---|---|
| **chord every** | Schedules a full chord change every 2, 4, 8, 16, 32, 64 or 128 bars — or **never** to hold your chord. The readout counts down to the next change. Default: 32 bars. |
| **note drift** | Small changes between full chords. Every 2 bars it may slide a held note to a nearby scale note, and sometimes add or remove a note (keeping 3–6). 0% = the chord stays exactly as is. |
| **NEW CHORD** | Generates a new dark chord now and restarts the countdown (also the **G** key). |
| **CLEAR NOTES** | Releases all held notes. |

> Because timing is counted in bars, the tempo also affects how fast the harmony moves.

---

## 8. Arp (arpeggiator)

*Color: cyan.* Plays the held notes one at a time in a pattern.

### Sequence

| Control | Description |
|---|---|
| **arp** | Turns the arpeggiator on or off. |
| **pattern** | **up**, **down**, **pingpong** (up then down), **converge** (outside notes inward), **orbit** (circles around the *shape* of your dots on the grid), **random**, **drunk** (wanders back and forth). |
| **rate** | Note length: 1/4, 1/8, 1/8T, 1/16, 1/16T, 1/32 (T = triplet). |
| **octaves** | Repeats the pattern across 1–3 octaves. |

### Voice

| Control | Description |
|---|---|
| **voice** | The synth engine (see table below). |
| **timbre** | One knob that changes the character of the current voice. |
| **cutoff** | Brightness of the filter. |
| **resonance** | Filter emphasis / whistle. |
| **gate** | Note length, from short plucks to long legato. |
| **level** | Arp volume, 0–200%. |

| Voice | Sound | What **timbre** does |
|---|---|---|
| **acid** | Saw + square, squelchy | Mix of the square layer |
| **supersaw** | Five stacked detuned saws | Adds a sub octave |
| **fm** | Metallic, clangy | Modulator ratio (how clangy) |
| **pluck** | Short, snappy | Brightness of the pluck |
| **sine fold** | Smooth → gritty | Amount of wave folding |
| **chip** | 8-bit pulse (always bit-crushed) | Pulse width |
| **formant** | Dark, vocal | Vowel: *oo → oh → ah* |
| **glass** | Clean, bell-like | Amount of overtones |

### More ▸

| Group | Control | Description |
|---|---|---|
| shape | **attack** | Fade-in time of each note (0–300 ms). |
| shape | **detune** | Width/thickness from detuned layers. |
| shape | **filter env** | How much each note "wows" the filter open. |
| variation | **chaos** | Randomly skips notes and adds occasional octave jumps. |
| variation | **ratchet** | Chance a note splits into 2–4 rapid repeats (these are bit-crushed). |

---

## 9. Pad (drone + 2 LFOs)

*Color: blue.* A slow, detuned drone on the held notes, with a sub-bass underneath. When the chord changes, the pad crossfades smoothly.

### Drone

| Control | Description |
|---|---|
| **level** | Pad volume. |
| **filter** | Pad brightness (lower = darker). |
| **drift** | Detune and wobble of the pad voices, plus a very slow built-in filter sway. |
| **sub** | Level of the sub-bass on the chord's lowest note. |

### LFO 1 and LFO 2

Two low-frequency oscillators that move a pad parameter over time. Each has a small **scope** showing one cycle of its wave with a dot riding along it (random shapes show their recent steps).

| Control | Description |
|---|---|
| **target** | What it moves: **cutoff** (filter sweep, ±2 octaves), **resonance**, **volume** (tremolo), **pitch** (vibrato, up to ~±2.5 semitones), **pan** (left ↔ right), or **off**. |
| **shape** | **sine**, **triangle**, **square**, **saw**, **s&h** (jumps to a random level each cycle), **smooth random** (glides to random levels). |
| **sync** | **free** (use the rate knob) or locked to tempo: 1/8, 1/4, 1/2 bar, 1, 2, 4, 8 or 16 bars. |
| **rate** | Speed in free mode (from ~50-second cycles to ~12 Hz). Turning it switches sync back to *free*. |
| **depth** | How strongly it moves the target. |

Both LFOs can target the same parameter — their effects add together.

> **Note:** with *volume* as the target and a high depth on a slow LFO, the pad will fade almost to silence for several seconds each cycle. That is expected.

---

## 10. Drums

*Color: amber.* A classic 16-step, six-voice drum machine. The pattern itself is edited on the **drum strip** under the field.

### Machine

| Control | Description |
|---|---|
| **drums** | Turns the drum machine on or off. |
| **RANDOM BEAT** | Rolls a new pattern (kick on beat 1, snares mostly on 2 and 4, everything else scattered). |
| **CLEAR BEAT** | Empties the pattern. |

> A new random beat is rolled **every time you press Start** — unless you have just loaded a preset, in which case its beat is kept until you press *random beat*, *clear beat* or **R**.

### Selected drum

Pick a drum with the **KCK SNR CLP RIM CHH OHH** buttons (or click its name on the strip). These controls edit only that drum:

| Control | Description |
|---|---|
| **level** | Volume of this drum. |
| **tune** | Pitch, ±24 semitones. |
| **decay** | Length of the sound's tail. |
| **mute** | Silences this drum (its row dims on the strip). |

### Bus

| Control | Description |
|---|---|
| **bus drive** | Distortion on all drums together. |
| **swing** | Delays every second 16th for a shuffled groove. |
| **mutate** | Chance that the pattern changes by one step every 2 bars (mostly hats and rims). |

### More ▸ — drum envelope & sends

| Control | Description |
|---|---|
| **attack** | Fade-in of the selected drum (0–250 ms) — soft, swelling hits. |
| **delay send** | How much of the selected drum goes to the delay. |
| **verb send** | How much of the selected drum goes to the reverb. |

The closed hat **chokes** (cuts off) the open hat, like on a real drum machine.

---

## 11. Euclid (glitch percussion)

*Color: lime.* Five abstract percussion voices, each running its own **Euclidean rhythm**. A Euclidean rhythm spreads a number of hits (**pulses**) as evenly as possible across a loop (**steps**) — for example 3 in 8, 5 in 16, 4 in 13. Because each voice can have a different loop length, the voices drift against each other in polyrhythms.

### Rhythms display

Each voice is a colored ring of dots: lit dots are hits, the white dot is the playhead, and lines connect the hits into a shape. The center shows the selected voice and its *pulses/steps*. **Click a ring** to select that voice.

### Machine

| Control | Description |
|---|---|
| **euclid** | Turns the machine on or off. |
| **bus level** | Volume of the whole machine, 0–200% (default 200%). |
| **mutate** | Chance per bar that a rhythm changes slightly (adds/removes a pulse, rotates, or stretches its loop). |
| **NEW RHYTHMS** | New patterns for all voices; sounds are kept. |
| **RANDOMIZE** | New rhythms *and* sounds for all voices. |

### Selected voice

Pick a voice with **DUST · SHARD · BYTE · ZAP · GRAIN** (or click its ring). A short note under the buttons explains what *tone* and *sweep* do for the current engine.

| Control | Description |
|---|---|
| **engine** | The sound generator (see table below). |
| **rate** | Speed of this voice's steps: 1/4 to 1/32, including triplets. |
| **steps** | Loop length, 1–32. |
| **pulses** | Number of hits in the loop. |
| **rotate** | Shifts the pattern around the loop. |
| **pitch** | Base frequency (~30 Hz – 12 kHz). |
| **tone** | Engine-specific character (see table). |
| **decay** | Length of each hit (5 ms – 1.5 s). |
| **level** | Volume of this voice. |
| **mute** | Silences this voice. |

| Engine | Sound | tone | sweep |
|---|---|---|---|
| **noise** | Filtered noise burst | Filter shape/resonance (low → lowpass, high → highpass) | Filter sweep |
| **metal** | Inharmonic square cluster | How inharmonic | Pitch dive |
| **byte** | Chopped, stuttering pulse | Chop rate (slow stutter → buzz) | Pitch dive |
| **zap** | Laser sweep | Sine → saw | Laser direction and depth |
| **grain** | Cloud of tiny grains | Number of grains | Pitch scatter |
| **fm** | Clangy digital tone | Modulator ratio | Pitch dive |
| **crackle** | Random dust / static | Crackle density | Filter sweep |

### More ▸

| Group | Control | Description |
|---|---|---|
| feel | **prob** | Chance each hit actually plays. |
| feel | **ratchet** | Chance a hit splits into 2–4 rapid repeats. |
| feel | **pitch rand** | Random pitch variation per hit (up to ±2 octaves). |
| feel | **sweep** | Pitch or filter movement during the hit (−/+). |
| feel | **attack** | Fade-in time (0–100 ms). |
| color & space | **drive** | Distortion on this voice. |
| color & space | **crush send** | Amount sent through the bit-crusher. |
| color & space | **pan** | Stereo position. |
| color & space | **pan rand** | Random stereo spread per hit. |
| color & space | **delay send / verb send** | Effect sends. |
| color & space | **RANDOMIZE VOICE** | New sound and rhythm for the selected voice only. |

---

## 12. Break (break chopper)

*Color: yellow.* An **Amen-style breakbeat**, synthesized from scratch (it is *not* a sample of the original recording), which is recorded into a buffer and then sliced and re-arranged live, jungle-style.

**The break chopper is OFF by default** — switch **break** on to hear it. You may want to turn the regular drums off while it plays.

### Break display

The waveform shows the break with a grid of 16th-note slices (bright lines = bars). As it plays, slices flash in the color of what happened to them:

| Color | Chop type |
|---|---|
| Yellow | straight (played in order) |
| Orange | jump |
| Cyan | stutter |
| Red | reverse |
| Purple | roll |
| Green | pitch |
| Grey | gap |

The white marker at the bottom is the current position in the loop. The status line says when the break is ready or re-rendering.

### Chopper

| Control | Description |
|---|---|
| **break** | Turns the break chopper on or off. |
| **level** | Volume, 0–200%. |
| **chop** | How often a slice gets mangled instead of played straight. |
| **chop mode** | **live (fresh)** = new chops every pass; **loop 1 / 2 / 4 bars** = a chop pattern that repeats. |
| **source** | Which part of the break to chop: bar 1 only, bars 1–2, or all 4 bars. |
| **pitch→bpm** | **On:** the break's pitch follows the tempo, like old jungle samplers (slow tempos = deep and dark). **Off:** original pitch; at slow tempos slices play with gaps or overlaps. |
| **NEW CHOPS** | Re-rolls the looped chop pattern. |
| **RAND CHOPPER** | Randomizes the chop settings. |
| **RAND KIT** | Randomizes the drum kit and grit, then re-renders the break. |

### More ▸

**Chop types** — how likely each mangle is when a chop happens:

| Control | Effect |
|---|---|
| **jump** | Plays a different slice of the break |
| **stutter** | Repeats the previous slice |
| **reverse** | Plays the slice backwards |
| **roll** | Rapid 2–4× retrigger |
| **pitch** | Shifts the slice ±5, 7 or 12 semitones |
| **gaps** | Silence |
| **gate** | Cuts slices shorter for a tighter, choppier sound |

**Kit** — the synthesized drums inside the break:

| Control | Description |
|---|---|
| **kick tune / kick decay / kick punch** | Pitch, length and attack click of the kick |
| **snare tune / snare snap / snr decay** | Pitch, noise "snap" and length of the snare |
| **ghosts** | Volume of the quiet ghost-note snares |
| **ride tone / ride decay / ride level** | Brightness, length and volume of the ride |
| **swing** | Shuffle inside the break |
| **room** | Small-room reverb baked into the break |

**Grit** — old-sampler character, applied to the rendered break:

| Control | Description |
|---|---|
| **saturate** | Warm to heavy distortion |
| **bit depth** | 4–16 bits (lower = crunchier) |
| **samp rate** | Sample-rate reduction (down to ~5.5 kHz) |
| **vinyl** | Crackle and hiss |

**Mix:** **lowpass**, **highpass**, **delay send**, **verb send**.

> Changing any **kit** or **grit** control re-renders the break in the background (a fraction of a second) without stopping the music.

---

## 13. Orbs

*Color: red.* Controls how orbs move and what they sound like.

### Field

| Control | Description |
|---|---|
| **energy** | Orb speed — and how many orbs auto-spawn. |
| **auto-spawn** | When on, new orbs drift in occasionally (they fade out after a while). |
| **+ ORB** | Adds an orb (also the **O** key). |
| **CLEAR ORBS** | Removes all orbs (also the **C** key). |

### Sound

| Control | Description |
|---|---|
| **voice** | **mix** (each orb gets its own random voice), or one voice for all: **metal**, **bell**, **glass**, **zap**, **stutter**, **grain**, **drop** (deep tom-like hit), **void** (dark resonant sweep). |
| **pitch** | Transposes orb hits ±24 semitones. |
| **decay** | From tiny clicks to long ringing tails. |
| **tone** | Brightness / intensity of the voice. |
| **level** | Orb volume. |

### More ▸

| Group | Control | Description |
|---|---|---|
| detail | **oct spread** | How often a hit jumps up or down an octave. |
| detail | **attack** | Fade-in of orb hits (0–200 ms). |
| detail | **collisions** | Volume of orb-on-orb pings and wall thuds (0 = silent). |
| sends | **crush send / delay send / verb send** | Effect sends for all orb sounds. |

---

## 14. Glitch

*Color: purple.* Random digital damage on top of everything.

| Control | Description |
|---|---|
| **amount** | How often glitch events happen: tape-warp moments on the delay (echoes bend in pitch), bit-crushed arp notes, crushed ticks, and visual screen tears on orb hits, snares and claps. |
| **ticks** | Tiny random clicks and crackles on the 16th-note grid, with occasional fast stutter rolls. |
| **crush** | Bit depth of the shared bit-crusher (1–8 bits; lower = harsher). It affects everything sent to it: crushed arp notes and the *chip* voice, orb crush sends, Euclid crush sends, and ticks. |
| **pulse** | A deep, distorted sub thump: always on beat 1, often beat 3, sometimes others. Off by default; adds weight under the drums or works as a minimal beat on its own. |

---

## 15. Master FX

*Color: grey.* Effects shared by the whole instrument.

| Control | Description |
|---|---|
| **reverb** | Return level of a long, dark reverb. |
| **delay** | Return level and feedback of a tempo-synced (dotted-8th) delay. |
| **distortion** | Parallel saturation over the whole mix. |

The amount each module sends to the reverb and delay is set in that module's own controls.

---

## 16. Presets and sharing

### Saving and loading

- **Save:** press **SAVE**, then click a slot (or press **Shift + 1–8**).
- **Load:** click a filled slot (or press **1–8**).
- **Clear:** right-click a slot.
- Hover a slot to see its name (key, scale and tempo, e.g. `E phryg 78`) and when it was saved.

**A preset stores:** key, scale and held notes; all arp, pad and LFO settings; the drum pattern and every drum's settings; every Euclid voice's rhythm and sound; the break chopper and kit; orb sounds; glitch and master effects.

**A preset does not store:** master volume (so loading never blasts you) or the orbs currently on screen.

Slots are saved in your browser, so they survive closing the page — but only in that browser on that device, and clearing browser data removes them.

### Share codes

1. Click **SHARE → COPY CODE**. The whole setup is copied to your clipboard as a text code (if the clipboard is blocked, the code appears in the box for you to copy).
2. To load a code, paste it into the box and click **LOAD**.

Codes work in any browser and on anyone's copy of NULL·FIELD. For setups you really love, keep a copy of the code somewhere safe.

---

## 17. Keyboard shortcuts

| Key | Action |
|---|---|
| **Space** | Start / stop |
| **G** | New chord |
| **O** | Add an orb |
| **C** | Clear orbs |
| **R** | Mutate all (randomize everything) |
| **1 – 8** | Load preset slot |
| **Shift + 1 – 8** | Save to preset slot |
| **Arrow keys** | Adjust the focused knob |

---

## 18. Tips and recipes

- **Freeze and play.** Set tempo to 0 and throw orbs: the pad drones and the orbs become the only rhythm.
- **Jungle mode.** Turn the regular drums off, switch the break on, set *chop mode* to *loop 2 bars* with chop around 50%, and add the Euclid machine at a lower level on top.
- **Polyrhythm overload.** Set Euclid voices to triplet rates (1/16T) while the drums stay on straight 16ths.
- **Steady drone.** Set *chord every* to *never* and *note drift* to 0, then shape the pad with slow LFOs on cutoff and pan.
- **Watch mode.** Press **▾ hide** to collapse the dock and let the field play full-screen.
- **Explore safely.** Save to a slot, press **R** a few times, and reload the slot if you get lost.

---

## 19. Troubleshooting

| Problem | What to try |
|---|---|
| **No sound** | Click *Enter the field* or *Start*. Check that the browser tab isn't muted and the **MASTER** knob is up. Some modules (break, pulse) are off by default. |
| **The pad keeps fading out** | An LFO is probably targeting *volume* with high depth — lower its depth or change its target. |
| **Sound cut out briefly with a glitch flash** | NULL·FIELD noticed unstable audio and automatically rebuilt its effects. Playback continues on its own. |
| **Knobs make test sounds** | Turn **preview** off in the dock tools. |
| **Preset slots are empty after returning** | Slots live in browser storage; private browsing or clearing site data removes them. Use share codes to back up favorites. |
| **Everything is too busy** | Lower *energy* (orbs), *ticks* and *amount* (glitch), Euclid *bus level*, or switch modules off from their tabs. |
| **Small screen feels cramped** | Use **▾ hide** to collapse the dock while playing. NULL·FIELD works best on a wide screen. |
