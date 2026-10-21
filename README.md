# Sega Rally Revo (PC) — Frame Pacing Fix P1

An **unofficial, free and offline community patch** intended to address uneven frame delivery and microstuttering in *Sega Rally Revo (2007)* on Windows PC.

## Supported executable version

**SEGA Rally.exe — file version 4.0.6.0** (Windows PC). This patch is tied to the exact original **SHA-256 hash** documented below; the version number alone is not enough to confirm compatibility.

## Download

Once uploaded, get the official package from [Releases](https://github.com/Martijnsx/Sega-Rally-Revo-Frame-Pacing-Fix/releases). The ZIP includes **SRR_P1_Patcher.html**, source code, Python alternative, checksums and technical documentation. It contains **no copyrighted game EXE or DLL**.

## How to install (Windows)

1. Download and **extract the ZIP** to a folder.
2. **Unblock the downloaded file in Windows Explorer if necessary:** right-click `SRR_P1_Patcher.html` → **Properties** → **General** → tick **Unblock** (if present) → **Apply**. You can also unblock the downloaded ZIP *before* extracting it. Do this only for a download whose origin you trust and have verified.
3. Open **SRR_P1_Patcher.html** in a desktop web browser. It works **offline**.
4. Select your own **SEGA Rally.exe**. The patcher checks its hash and refuses unrecognized versions.
5. Click **Download patched EXE**. Close the game, **back up your original EXE**, and put the downloaded copy in the game folder as `SEGA Rally.exe` (remove any browser-added `(1)` suffix).
6. If Windows marks the resulting EXE as blocked, use its **Properties → General → Unblock** option too, but only if you've verified the file.
7. Launch the game normally. To undo the fix, use your backup or the patcher's **Download restored EXE** feature.

**Do not disable antivirus or Windows security protections to use this patch.** If an Unblock checkbox is absent, no action is required.

## What P1 changes

The patch adjusts two timer initializers from 15,999 microseconds to zero; it changes **four bytes in total**. It does not modify renderer quality, simulation step, DLLs, network code or game content.

Only the following original build is accepted:

- **File version:** `4.0.6.0`
- **Original EXE SHA-256:** `246b4a6338d8f40069d4a24bc35073c6b5649bc71df3d2d6238139e07112db39`
- **Patched EXE SHA-256:** `d1a1a2737b71ea4edfb46bc8bcdc712bf55485d521f7e284be5b93df1512d9e7`
- **EXE size:** 3,700,786 bytes

The initial tester reported improved frame pacing, but this is not a multi-system benchmark. Unknown or modified EXEs are not supported.

## A lot of trial and error — buy me a coffee? ☕

Getting to a working candidate took **a lot of trial and error**. I tried **multiple times with different AI models**, exploring, testing and revisiting ideas until we finally found an adjustment that seems to fix the stuttering on my system. It was far from a one-click solution.

**This fix is and will remain completely free.** If it helped you enjoy Sega Rally Revo again, I would really appreciate it if you could [**buy me a coffee on Ko-fi**](https://ko-fi.com/martijnsx) — for example **€5**. Any support is appreciated, but **donations are entirely optional**. Thank you!

## Feedback and issues

Report your game edition, EXE hash, operating system, GPU, display refresh rate, FPS limit and before/after results in [Issues](https://github.com/Martijnsx/Sega-Rally-Revo-Frame-Pacing-Fix/issues). Do not upload copyrighted game executables.

## Technical details

The downloadable package includes `TECHNICAL.md`, `patch.json`, readable source code, and test scripts. It also contains exploratory renderer research, **not** an additional renderer modification.

## Disclaimer

Unofficial fan project; not affiliated with or endorsed by SEGA or the game's developers or publishers. Trademarks belong to their respective owners. Back up your original files. Use at your own risk.
