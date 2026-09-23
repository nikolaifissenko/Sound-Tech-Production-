# Release specs — singles for Spotify & DSPs

## Loudness
- Spotify normalises to -14 LUFS integrated (default). Apple Music ~-16 LUFS. YouTube ~-14 LUFS.
- A master louder than that is simply turned down — you gain nothing except lost dynamics.
- Realistic alt-rock target: **-9 to -11 LUFS integrated**, short-term peaks in choruses a bit higher.
  Going to -7 buys nothing on streaming and costs punch.
- **True peak ≤ -1.0 dBTP** (≤ -2.0 dBTP if the master is louder than -10 LUFS: lossy encoding adds overs).
- Measure: `ffmpeg -i master.wav -af ebur128=peak=true -f null -`

## Delivery formats
- Master: WAV, 24-bit, 44.1 kHz (or 48 kHz if the distributor accepts it), stereo.
- No dither if staying 24-bit; dither once only when reducing to 16-bit.
- Leave 0.5–1 s of silence/tail at the end, trimmed start (no dead air before the downbeat).
- Keep a 16-bit/44.1 version for CD/Bandcamp if needed.

## Stems to archive per single
Drums, Bass, Guitars, Keys/Synths, Lead Vox, BVs, FX — each from bar 1, same length, no master bus processing. Plus an instrumental and an a cappella (useful for sync, remixes, TikTok/Reels edits).

## Pre-release checklist
- [ ] Mix approved by the whole band on at least 3 systems (monitors, phone, car)
- [ ] Mono check: vocal and kick/snare/bass survive
- [ ] Loudness + true peak measured and within spec
- [ ] Master A/B'd against 2 loudness-matched references
- [ ] First 10 seconds grab attention (playlist editors and listeners skip fast)
- [ ] ISRC assigned, metadata (credits, composers, producers) correct
- [ ] Instrumental + a cappella + stems exported and backed up
- [ ] Short-form edit (15–30 s hook) cut for Reels/TikTok
- [ ] Delivered to distributor ≥ 4 weeks before release (Spotify editorial pitch needs ~7 days minimum, more is better)
