# Sea Shanty 2 Dance Mod - Changelog

## [1.3.0] - 2026

### Added

- A level-up sound effect when any of your skills gains a level. It plays only for
  you and is not positional, so nobody else hears it
- A "Shanty4Heim Level-up Sound" checkbox in Settings > Audio, directly under the
  volume slider, for switching it off. Stored as `LevelUpSound` in the config file

### Changed

- The level-up sound runs through the Shanty4Heim Sound slider, so one volume
  covers everything the mod plays

### Fixed

- The shanty only responds to the dance emote now. Sitting down on a boat used to
  start the whole track, and every one-shot emote set off a second or two of it

## [1.2.1] - 2026

### Fixed

- Other players dancing on a boat now reliably starts the music on your client
- Removed the custom RPC layer entirely; emote state is read from the synced ZDO, so playback no longer depends on RPC registration winning a race at spawn time
- Ship detection now works for remote players, not only for yourself

### Changed

- Several dancers at once share a playback position instead of drifting out of phase
- Tracks re-encoded to mono 32 kHz, cutting the download from roughly 24 MB to 8 MB

### Added

- A "Shanty4Heim Sound" volume slider in Settings > Audio, directly under Music
- Volume setting in the config file, kept in sync with the slider

## [1.1.0] - 2025

### Improvement

- Modified instances to be player based
- Added player audio object, rather than global audio
- Multiple player instance issue fixed

## [1.0.3] - 2025

### Fixed

- Fixed incorrect use of RPC Handlers

## [1.0.2] - 2025

### Fixed

- Fixed multiplayer synchronization so all players hear the sea shanty when any player dances on a boat
- Added RPC handlers to properly sync music across clients
- Fixed audio playback in multiplayer sessions

## [1.0.1] - 2025

### Fixed

- Improved audio loading reliability
- Better error logging for debugging resource loading issues

## [1.0.0] - 2025

### Added

- Initial release of Sea Shanty 2 Dance Mod
- Sea shanty plays when player performs emote on a boat
- Local audio playback with loop support
- Integration with Valheim's emote system
