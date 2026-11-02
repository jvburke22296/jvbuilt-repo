# JVBuilt 6.4.11

Garage 2.0.9.17 selects available English subtitles at the start of each movie or episode, including playback resolved through TMDB Helper. If English is unavailable, playback continues with subtitles off. A short startup retry handles subtitle tracks that appear late.

## Update Garage first

Update JVBuilt's Garage to 2.0.9.17 or later and restart Kodi before installing this build. Older Garage installers perform a full profile reset.

The new Android and Windows installers stage and verify the incoming build, preserve the current device's personal configuration, then activate the prepared update. Device identity, accounts, sources, favourites, libraries, profiles, backup settings, native playback add-ons and installed add-ons absent from the incoming build are retained. The selected build's performance defaults and version remain current. SQLite data is copied consistently, and Android copies avoid restricted filesystem attributes. The previous Kodi directory is retained outside the active profile for recovery, so allow storage for both copies.

## Hardware profiles

| Profile | RAM cache | Widget/hub items | Artwork / fanart | Read factor |
|---|---:|---:|---|---|
| PC OptiPlex 3050 | 256 MB | 25 | 720 / 1080 | Adaptive |
| Fire TV Stick 4K | 128 MB | 12 | 540 / 1080 | 4x |
| SonTV / lower-memory Fire TV | 64 MB | 8 | 360 / 720 | 2x |

The home label reads the configured Kodi device name instead of embedding a TV identity. Two inherited workstation-specific TMDB discovery icon paths now use portable special://home paths. The existing intro, blue/cyan theme and live-delay behavior are retained.

The shared service can export Android Kodi logs locally for a separately configured collector. Upload destinations, schedules, TV registries, logs, accounts and backups are not bundled in this release.

## Validation

An Android device completed a full 6.4.10-to-6.4.11 update and reopened with its personal configuration, performance settings and native playback add-ons intact. Before and after the update, live playback tests confirmed English enabled, non-English-only subtitles disabled, and English re-enabled on the next playback. Saved configurations from seven installations passed separate preservation simulations. The Windows activation path and rollback were exercised with staged fixtures. The final publication adds portable icon paths and release metadata; the tested playback and preservation code is unchanged.
