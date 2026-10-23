# Provenance — Tanpura recordings (Freesound, luckylittleraven, CC0)

The four AAC files in this folder are **edited derivatives** of recordings published by **luckylittleraven** on
[Freesound](https://freesound.org) under **Creative Commons 0 1.0** (public-domain dedication,
https://creativecommons.org/publicdomain/zero/1.0/; each sound's page states "You can copy, modify, distribute and perform the
sound, even for commercial purposes, all without the need of asking permission to the author"). Downloaded by the founder on
2026-10-02 from the pack "Tanpura C Sharp" (https://freesound.org/people/luckylittleraven/packs/23512/). Attribution is not
required; this file is our courtesy credit and our evidence of provenance. No endorsement by the author is implied.

| File in this folder | Freesound sound | Page |
|---|---|---|
| tanpura-pa-dha-sa-sa-01.m4a | 416595 — Tanpura Pa-Dha-sa-Sa 01 C sharp.wav (19.5 s) | https://freesound.org/people/luckylittleraven/sounds/416595/ |
| tanpura-mournful-bass-line.m4a | 416596 — Tanpura Mournful Bass Line C sharp.wav (20.7 s) | https://freesound.org/people/luckylittleraven/sounds/416596/ |
| tanpura-pa-sa-sa-sa-03.m4a | 416583 — Tanpura Pa-sa-sa-Sa 03 C sharp.wav (22.6 s) | https://freesound.org/people/luckylittleraven/sounds/416583/ |
| tanpura-pa-sa-sa-sa-01.m4a | 416585 — Tanpura Pa-sa-sa-Sa 01 C sharp.wav (74.0 s) | https://freesound.org/people/luckylittleraven/sounds/416585/ |

## Processing (what differs from the originals)

`herramientas/preparar-muestras.sh` (ffmpeg 6): trimmed to 10 ms before the onset, peak-normalised to −3.0 dBFS, 0.6 s fade-out;
then (`FORMAT=aac`) down-mixed to mono and encoded as AAC 128 kbps (`ffmpeg -ac 1 -c:a aac -b:a 128k`): the shipped files peak at
−0.8…−1.2 dBFS after encoding (the limiter in the app keeps the headroom), and the four passages weigh 2 206 760 bytes from
24.1 MB of WAV originals; the SHA-256 table below identifies exactly what ships. Tuning measured with `herramientas/analizar-muestra.mjs`
and a low-band peak check: strings at C#3, C#4, C#5 and G#4 (Sa = C#4, midi 61); the app plays them one semitone up (D).

## SHA-256 of the originals (WAV 44.1 kHz 16-bit stereo, as downloaded 2026-10-02)

| Sound | SHA-256 |
|---|---|
| 416595__luckylittleraven__tanpura-pa-dha-sa-sa-01-c-sharp | 3aa44eb27dab5ebe8b14e9f12731357b54f5c423977a9e97b8912811791b7221 |
| 416583__luckylittleraven__tanpura-pa-sa-sa-sa-03-c-sharp | 01fe28e867db57bf8c5a9d0759f74bbeda3a996e562eed8774129c6e2690e2ca |
| 416585__luckylittleraven__tanpura-pa-sa-sa-sa-01-c-sharp | 092ba0fa3906b4944941e906156841fb8ace91b3d038285fa37d6770d07679ef |
| 416596__luckylittleraven__tanpura-mournful-bass-line-c-sharp | 43a28e9af1ef6ffa4c13fa3549bbe23555a2b3cefc6e030c7cae821d25ef59e7 |

## SHA-256 of the files in this folder (frozen 2026-10-02)

| File | SHA-256 |
|---|---|
| tanpura-mournful-bass-line.m4a | e7848c2c11de3d5d7cd34c6726a15a541bebb6f19842a71ef4302dcf62aefd8a |
| tanpura-pa-dha-sa-sa-01.m4a | 367a21fae9a52602ab90a566a3e65adae0dad437a583997cfc9eee9e7ca1ce66 |
| tanpura-pa-sa-sa-sa-01.m4a | 07080113f871da614f951e7b75ea6024947fa0f3405f159efd8411fc9b74a9b1 |
| tanpura-pa-sa-sa-sa-03.m4a | bd6890af1edffbe6fb4433968bc01732c8eb424134a46d3069198ab9c7d41b0e |
