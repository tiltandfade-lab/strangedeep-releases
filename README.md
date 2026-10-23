# Strangedeep releases

Release files for Into the Strangedeep, written by `tools/release/publish.sh` in the game's repository. No source lives here.

- `latest.json`: the newest version per platform and its manifest's sha256.
- `manifests/<version>.json`: every file of that release (path, size, sha256, executable bit, chunks).
- `objects/<sha256>`: file contents, and the 64 MiB chunks of bigger files, named by their sha256.

The game downloads these from `https://raw.githubusercontent.com/tiltandfade-lab/strangedeep-releases/main/` with no login. Each publish replaces this branch with one commit holding the latest two releases, so this repository keeps no history.
