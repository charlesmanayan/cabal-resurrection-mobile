# CABAL RESURRECTION — mobile test client

Android launcher and release channel for the operator's EP36 test server.

## Current status

The tested engine is x86_64. An ARM64 phone port is not ready. No verified automatic-download APK release has been published yet.

Verified in the original lab: login, character selection, movement/combat, outgoing whisper, buddy acceptance, party join/member updates, and outgoing party chat. General auto quest and additional game systems remain under test.

## Planned distribution

- Versioned, signed test APKs in GitHub Releases.
- A version/checksum manifest used by the Android updater.
- Automatic native-library and game-data downloads from the EP36 test host.
- Android's normal installation confirmation for APK updates.

Only selected launcher source and release metadata belong in this repository. Account passwords, PINs, session tokens, server administration credentials and signing keys must not be committed.

This repository does not contain the original game's full source project.
