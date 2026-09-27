# Suzuka‘s TX-41enhancement v1.1.0

A Helldivers 2 TX-41 Sterilizer mod for Bingus Shared Loader v15+ (API 1).

## Features

- One-handed use with PDW grip type while retaining the original firing animation.
- Magazine capacity: 175 rounds.
- Gas damage immunity while carrying the TX-41.
- Gas and confusion application values: 100 each on hit.

## What changed in v1.1.0

When a verified local player equipment record remains stable and does not contain a confirmed TX-41 entity, Gas Guard skips repeated full snapshots. A changed or unreadable record, or a changed mission context, resumes identification. Active effects still receive validation and are restored on unequip. Identity checks, unique matching, readback verification, and fail-closed writes remain in place.

## Download

Download the ZIP from the [latest release](https://github.com/Suzuka2788/helldivers-2-tx41-enhancement/releases/latest) and install it through your mod loader.

## Verification

The v1.1.0 package passed offline syntax, identity, simulated write and restore, and ZIP integrity checks. It has not yet been verified in game. For Gas Guard, inspect `SuzukaSterilizerGasGuard.log`: `LOCAL_ABSENT_SKIPS`, `FULL_SCANS`, `PERF_WATCH`, `PERF_SNAPSHOT`, `STERILIZER`, and `WRITES`. For status application, inspect `SuzukaTX41Status100.log`: `PATCH`, `reads`, `bytes`, and `writes`. Compare any stutter to frame time; fewer scans alone do not prove a stutter is fixed.

SHA-256 (`Suzukas-TX-41enhancement-v1.1.0.zip`): `4656015396758463B16621C2E22DFB4C3932E3B1E750849A5C80340E566B6DB5`.
