Updates `DeCiv 2` from the repository pinned in `mods-manifest.json`.

Changed files:

- docs/mod-attribution/deciv-2.md
- docs/mod-attribution/forgotten-factions-for-deciv.md
- docs/mod-attribution/outlaws-of-the-wastes.md
- docs/mod-attribution/steampunk-nations-for-deciv.md
- mods-manifest.json

Validation run in this workflow:

- `python tools/mods/mod_repo_manager.py update-one --mod "deciv-2" --dry-run`
- `python tools/mods/mod_repo_manager.py generate-reciv-vanilla`
- `./gradlew check`
- `./gradlew :android:assembleDebug`
