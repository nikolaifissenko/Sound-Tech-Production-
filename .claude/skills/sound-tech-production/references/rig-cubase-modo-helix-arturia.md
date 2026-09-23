# Rig notes — Cubase + MODO DRUM + Helix + Arturia

Map generic advice to these tools. Check `sessions/setup.md` for the Cubase edition.

## Cubase stock tools (Pro unless noted)
| Job | Plugin |
|---|---|
| Surgical / dynamic EQ | Frequency 2 (dynamic bands + sidechain, e.g. duck gtrs 2–3 kHz from vocal) |
| Quick EQ + comp | Channel strip (every channel, all editions) |
| Peak comp (FET-ish) | Vintage Compressor / Tube Compressor |
| Leveller / bus glue | Compressor, Bus Compressor (Cubase 13+), Standard Compressor |
| De-ess | DeEsser |
| Reverb | REVerence (convolution), RoomWorks, Shimmer |
| Delay | MonoDelay / StereoDelay (tempo-synced) |
| Saturation | Magneto II, Tape Saturation |
| Loudness / true peak | SuperVision (LUFS + true peak modules), Control Room loudness meter |
| Mono check | Control Room mono button, or MixConvert |
| Tuning / timing | VariAudio (Pro), AudioWarp / Hitpoints |
| Imaging/Master | Maximizer, Imager (Pro), MultibandCompressor |

Workflow habits:
- Use Group channels for buses (Drums, Bass, Gtrs, Vox, FX) and FX channels for shared reverbs/delays.
- Pre-fader sends only when you need independent return levels; default post-fader.
- Export: File → Export → Audio Mixdown, WAV 24-bit, 44.1/48 kHz; "Channel Batch Export" for stems.
- Mixer snapshots / project versions before big changes.

## MODO DRUM (IK Multimedia)
- Physically modelled: no mic bleed or real phase problems, but it can sound **too clean and too even**.
- Humanise: vary velocity (±5–15), avoid identical hits on snare/hats, nudge timing a few ms on fills. Use MODO's own velocity-to-strike-position modelling.
- Route **multi-out** into Cubase (kick, snare, toms, OH, room separately) so you mix drums like a real kit — don't mix only the stereo out.
- Its room/OH mics are where realism comes from: parallel-crush the room.
- Consider layering a kick/snare sample (Groove Agent) only if MODO lacks attack in the mix.
- Tune kit to the song key (kick/toms tuning in MODO) — big improvement for low end with bass.

## Line 6 Helix (guitars, maybe bass)
- **Always record a clean DI track in parallel** with the Helix-processed track (Helix USB gives multiple inputs; or use Helix Native on the DI). Lets you re-amp at mix time instead of being stuck with the tone.
- Fizz/harshness in direct amp sims: tighten with the cab/IR block — high cut ~6–8 kHz, low cut ~80–100 Hz inside the preset; try a different IR before EQ'ing in Cubase.
- Doubles: record the part twice (real performance), consider a different amp/cab or IR on the second side for width.
- Less gain than you think: amp sims stacked double-tracked get muddy and small with too much drive.
- Bass: Helix bass amp + a DI blend; time-alignment is not an issue inside Helix but check against any separate DI.
- Set Helix output level so peaks land ~-10 dBFS in Cubase.

## Arturia
- V Collection synths/keys: HPF generously (pads/keys under 150–250 Hz fight guitars and bass), keep pads mono-ish or narrow unless they're a feature.
- FX Collection (if owned): Pre 1973 / TridA / V76 preamps for colour on vocals/bus; Comp FET-76 for vocal peaks; Comp VCA-65 for bus glue; Rev Plate-140 for vocal plate; Tape MELLO-FI for lo-fi effect.
- Check exactly which Arturia bundle is owned before recommending a specific Arturia plugin.
