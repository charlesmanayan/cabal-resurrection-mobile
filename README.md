# CABAL RESURRECTION mobile — EP36 testing

[Download the x86_64 test prerelease](https://github.com/charlesmanayan/cabal-resurrection-mobile/releases/tag/v0.17.0-lab-x86_64)

This prerelease is for compatible x86_64 Android emulators. The ARM64 phone port is in progress; a phone build has not been validated or released.

## Install

1. Download `CABAL-RESURRECTION-x86_64.apk` from the release assets and install it.
2. Open CABAL RESURRECTION. Allow approximately 20 GB of free space for initial setup. The app automatically downloads about 5.7 GB and installs about 11.4 GB of game files.
3. Interrupted downloads resume when reopened. Files and the game library are checked with SHA-256 before Play is enabled.
4. Use the privately provided EP36 lab account for EpMobile01. The current bridge accepts the dedicated moblab-prefixed account. Use one test session at a time.

Credentials, PINs and signing keys are never included in this repository. Future APK updates use Android's normal installation approval. Library updates reuse installed game data when its checksum is unchanged.

## Verified

Clean installation on an Android 15 x86_64 emulator, interrupted-download recovery across APK updates, archive verification/extraction, library-only update, normal server authentication, EpMobile01 character loading, Bloody Ice world entry and touch-joystick movement. App installation and the login bridge required no root access. Software rendering (`swangle`) was used for world validation.

The login form contains Username, Password and Login only.

## Current limits

- ARM64 native compatibility work is ongoing. This APK contains x86_64 native code.
- The Android Studio host-GPU renderer produced a white title screen; the software renderer displayed the world. LDPlayer itself still needs testing.
- Some native UI text is clipped, and the native title still contains the previous branding.
- Incoming whisper display, mail and general autoquest remain unverified or incomplete. Earlier dedicated-character tests confirmed outgoing whisper, buddy acceptance, party joining and outgoing party chat.
- Compatibility adapters are currently validated for the dedicated lab character, not general accounts and characters.

This is an experimental test client, not a complete mobile port. It targets only the EP36 test environment. Production server configuration and databases were not changed for this release.
