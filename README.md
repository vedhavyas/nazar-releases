# nazar-releases

Release artifacts for [nazar](https://github.com/vedhavyas/nazar), the family's camera app.

Each release carries the desktop shell's signed update bundle (`nazar.app.tar.gz` and its `.sig`) and `latest.json`, the manifest every installed app reads to update itself. The Android APK lands here the same way once that shell ships.

This repository is public on purpose: the update check runs from wherever the app is, outside the household's WireGuard mesh, and GitHub release assets of a private repository are not reachable without a token. It holds no source and no secrets - the source lives in the private repository, and the artifacts are the same client binaries the app ships anyway.
