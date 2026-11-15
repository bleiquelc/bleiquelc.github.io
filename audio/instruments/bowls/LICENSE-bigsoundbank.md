# Provenance — Tibetan bowl recordings (BigSoundBank, CC0)

The four FLAC files in this folder are **edited derivatives** of recordings published by **Joseph Sardin** on
[BigSoundBank](https://bigsoundbank.com) under **CC0 1.0 Universal** (public-domain dedication by the author; the site's
licence page also offers WTFPL): https://bigsoundbank.com/licenses.html — "Adapt, remix, transform and create from material.
Use, including for commercial purposes. Without any restrictions. Without asking permission." Attribution is not required ("Nothing is mandatory, but
definitely appreciated"); this file is our courtesy credit and our evidence of provenance. Consulted and downloaded on
2026-10-02. No endorsement by the author or the site is implied.

| File in this folder | BigSoundBank sound | Canonical page |
|---|---|---|
| bowl-struck-1.flac | 1110 — Tibetan Bowl Struck #1 (31 s) | https://bigsoundbank.com/tibetan-bowl-struck-s1110.html |
| bowl-struck-2.flac | 2553 — Tibetan Bowl Struck #2 (14 s) | https://bigsoundbank.com/tibetan-bowl-struck-2-s2553.html |
| bowl-struck-3.flac | 2554 — Tibetan Bowl Struck #3 (10 s) | https://bigsoundbank.com/tibetan-bowl-struck-3-s2554.html |
| bowl-struck-4.flac | 2555 — Tibetan Bowl Struck #4 (14 s) | https://bigsoundbank.com/tibetan-bowl-struck-4-s2555.html |
| bowl-singing.flac | 1109 — Tibetan bowl singing (44 s) | https://bigsoundbank.com/tibetan-bowl-singing-s1109.html |

`bowl-singing.flac` was prepared the same way, but since 2026-11-15 it is not in this folder and does not ship with the app,
which does not use it. Its rows in this file still identify it.

## Processing (what differs from the originals)

`herramientas/preparar-muestras.sh` (ffmpeg 6): trimmed to 10 ms before the onset, peak-normalised to −3.0 dBFS, 0.6 s fade-out,
re-encoded as FLAC 16-bit mono 48 kHz. Re-running the script on the originals reproduces the same audio to within ±1 LSB of
rounding (an intermediate 24-bit pass preceded the 16-bit encode of the delivered files), not the same bytes: the SHA-256 table
below identifies exactly what ships. Root pitches measured with `herramientas/analizar-muestra.mjs`:
bowl-struck-2/3/4 = by pitch and session, the same bowl at 473–474 Hz (A#4 +25…30 cents), bowl-struck-1 and bowl-singing = a smaller bowl at 868–875 Hz (A5).

## SHA-256 of the originals as served by the site (FLAC, 2026-10-02)

| Sound | SHA-256 |
|---|---|
| 1110 | 7647b50940d484b7c757a62890a8259339005f8002856cb4dcf9d9989beeb488 |
| 2553 | 1abbf7f1867ac6086b0d0c8c01115f9551b3d273ebf8a5e7d459732afb5ead8f |
| 2554 | ad217c2f07484722c86876e587c2da3590ff557849acbde12a68b3e280955cbd |
| 2555 | 3cf3d0cff5b5279ef47dfaef74df1670ac2459a52a69f383b5d6db3be212f8c4 |
| 1109 | 010b51521394f18e076530787f26e1a11e496c986bc562a782abce102f1b78f7 |

## SHA-256 of the files in this folder (frozen 2026-10-02)

| File | SHA-256 |
|---|---|
| bowl-singing.flac | 6c0e304b686f7a60d8eba09340235d7bde079bbcb0b7a1baf4ac21554954c3c1 |
| bowl-struck-1.flac | 1963f3131d0de502a5de5b7c762622ee7990cb9cc712c051f2266d859e8c0a38 |
| bowl-struck-2.flac | 240c38916a5bdf529b763ec5ac4317e45e0a5c2e290259e94ebedb91fb79cf00 |
| bowl-struck-3.flac | 0ffb18fa5de61ddefd6bf01e60d5cf8dd039f65ee83cbecbcc8083aba8bf9590 |
| bowl-struck-4.flac | bf8a2c7a96ca4f7b2433e252b900a82d45a76d47283e44786db72601e0272d7f |
