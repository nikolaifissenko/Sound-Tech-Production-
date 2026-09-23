# Sound-Tech-Production

Nikolai's music production workspace for **Noble Sin** (alt rock, Rome, five-piece, female vocals).

## Rules
- Always use the `sound-tech-production` skill (`.claude/skills/sound-tech-production/`) for any request here.
- Read `sessions/setup.md` before giving tool-specific advice; translate advice into his actual tools
  (see `references/rig-cubase-modo-helix-arturia.md`).
- One log per song in `sessions/<song-slug>.md`, created from `sessions/_template.md`.
  Update it at the end of every working turn on that song.
- Audio files dropped in the repo can be analysed with ffmpeg/sox/Python (loudness, true peak, spectrum, mono).
  They are not preinstalled in the cloud container: `apt-get install -y ffmpeg sox` first.
- Avoid committing large audio (>50 MB); ask before committing any audio file.

## Rig (summary — full detail in `sessions/setup.md`)
Cubase · IK MODO DRUM · Line 6 Helix · Arturia.

## Status (last updated 2026-09-23)
- Skill, references, setup file and song template in place. No song in progress yet.
- **Next session starts with**: Nikolai describes the song he's making → create `sessions/<song-slug>.md`
  from the template and work from there.
- **Still to ask (once, then record in `setup.md`)**: Cubase edition (Pro/Artist/Elements),
  Helix hardware vs Native (and whether it's the audio interface), Arturia bundle (V Collection / FX Collection),
  vocal mic, monitors/headphones, self-recorded vs studio.
- Default branch is currently `claude/music-production-help-g5agfa`; could be renamed to `main` later.
