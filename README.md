# SEEKERTV

A spare Android phone as an office activity logger and security camera.
Pilot device: Solana Seeker, Byeongjeom office.

- Check in when you arrive: a photo is taken at once, then one every 30 minutes.
- Check out when you leave: the session closes and, later, security recording starts.
- Originals stay on the phone and are copied to the owner's own Google Drive.

Status: pilot, build A (device verification). See `docs/` for the specification.

## Build

Builds run on GitHub Actions (`.github/workflows/build.yml`). Each run publishes
its results to the `ci-out` branch: a short report, the tail of the build log,
unit test results and the unsigned release APK. The APK is signed afterwards
with the pilot key, which is never stored in this repository or on the build
server.
