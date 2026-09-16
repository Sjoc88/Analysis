# Multi-provider merge

Spotify JSON and YouTube Music Google My Activity HTML are parsed independently
and appended into `unified_listening_history`.

This is an event-level UNION, not a row-by-row match. Spotify track URIs and
YouTube video URLs are retained separately.

The supplied YouTube Music HTML provides timestamp, title, artist/channel and
video URL, but no playback duration. Therefore YT `ms_played` and
`minutes_played` are intentionally NULL.

`spotify_spotify_only_backup.db` preserves the Spotify-only database from
before the multi-provider merge.
