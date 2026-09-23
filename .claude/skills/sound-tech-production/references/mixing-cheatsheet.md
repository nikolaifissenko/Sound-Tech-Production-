# Alt-rock mixing cheatsheet (starting points, not rules)

## Gain staging
- Track at -18 dBFS average / peaks around -10 to -6 dBFS (24-bit, 48 kHz).
- Keep plugin inputs near -18 dBFS RMS; analog-modelled plugins misbehave hot.
- Mix bus peaking around -6 dBFS before mastering. No limiter on the mix you send to master.

## Drums
| Source | EQ | Compression |
|---|---|---|
| Kick in | HPF 30–40 Hz; weight 50–70 Hz; cut boxiness 300–500 Hz (-3/-6 dB); beater 2.5–5 kHz | 4:1, attack 10–30 ms (let the click through), release to tempo |
| Kick out/sub | LPF ~5 kHz; body 50–80 Hz | light or none |
| Snare top | HPF 80–100 Hz; body 150–250 Hz; ring cut (find it, narrow Q); crack 4–6 kHz | 4:1, attack 5–15 ms, fast release |
| Snare bottom | HPF 200 Hz; **flip polarity** vs top; sizzle 5–8 kHz | none, blend low |
| Toms | HPF 60–80 Hz; cut 300–500 Hz; attack 3–5 kHz; gate or edit bleed | 4:1 medium |
| Overheads | HPF 100–200 Hz (depends on how much kit they carry); tame 2–4 kHz harshness | light 2:1 or none |
| Room | HPF 80 Hz | crush it in parallel (10:1+, fast attack) and blend |

- Check phase: kick in/out, snare top/bottom, overheads vs snare. Align by nudging or with a phase tool.
- Drum bus: glue comp 2:1–4:1, attack 10–30 ms, auto/fast release, 2–3 dB GR. Parallel crush bus for energy.

## Bass
- DI + amp: time-align the amp to the DI (amp is typically 0.5–2 ms late).
- HPF 30–40 Hz. Fundamental 60–100 Hz. Cut mud 200–300 Hz. Growl/definition 700 Hz–1.5 kHz, clack 2–4 kHz.
- Compress 4:1, 3–6 dB GR; consistent level matters more than tone.
- Decide who owns the sub: kick or bass. Sidechain bass to kick (1–3 dB duck) if they fight.
- Keep low end mono below ~120 Hz.

## Guitars (rhythm)
- Double-tracked, hard-panned L/R (real doubles, not copies + delay).
- HPF 80–120 Hz. LPF 8–12 kHz. Cut 200–400 Hz mud and 2.5–4 kHz fizz/harshness if needed.
- Usually little compression — distortion is compression already.
- Leave a hole at 1–3 kHz for the vocal (dynamic EQ keyed from vocal works well).
- Leads: mono, centre-ish or opposing the vocal, delay > reverb.

## Female lead vocal
Typical chain: clean-up → EQ → comp 1 → de-ess → comp 2 / saturation → sends.
- HPF 80–120 Hz (higher if the voice is light).
- Cut boxiness 300–600 Hz; nasal 800 Hz–1.2 kHz if present.
- Presence 2–5 kHz (careful: harshness lives here too). Air shelf 10–12 kHz.
- Comp 1 (FET-style): fast, 4:1, 3–6 dB GR catches peaks. Comp 2 (opto-style): slow, 2–3 dB GR, levels phrases.
- De-esser 5–9 kHz — set by ear on "s" and "t".
- Ride volume (automation) before over-compressing. The vocal must read on phone speakers.
- Sends: short plate/room (1–1.5 s, predelay 20–40 ms) + 1/8 or 1/4 note delay, both HPF/LPF'd.
- Doubles/harmonies: HPF higher, tuck 6–10 dB under lead, pan wide.

## Space and depth
- Two or three shared reverbs (short room, plate, long hall), not one per track.
- EQ every reverb return: HPF 200–400 Hz, LPF 6–8 kHz, keeps the mix clean.
- Delay is less smeary than reverb for vocals in dense rock.

## Mix bus
- Gentle glue comp: 2:1, attack 10–30 ms, auto release, 1–2 dB GR.
- Optional tape/console saturation. No limiter when bouncing for master.

## Symptom → likely cause
| Symptom | Check first |
|---|---|
| Muddy | 200–400 Hz build-up across guitars/bass/keys; too much reverb; HPFs missing |
| Harsh / fatiguing | 2–5 kHz on guitars, cymbals, vocal presence boost; over-distorted gtrs |
| Thin | Over-HPF'd guitars; bass too low vs kick; phase cancellation |
| Small / not punchy | Over-compressed; transients killed by fast attack; no dynamics between sections |
| Vocal buried | Guitars occupy 1–3 kHz; no volume automation; reverb too wet |
| Great on headphones, bad on speakers/car | Low end (sub) imbalance, stereo tricks; check mono and a small speaker |
| Loud but lifeless master | Over-limiting; aim lower LUFS, keep crest factor |

## Monitoring hygiene
- Mix around 75–80 dB SPL; check quiet, check mono, check phone, check car.
- Reference against a loudness-matched commercial track every 20–30 min.
- Take breaks; ears flatten after ~45 min of loud work.
