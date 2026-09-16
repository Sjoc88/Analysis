# Spotify Data Quality Report

- JSON files: 11
- Total events: 62,581
- Track events: 62,517
- Podcast events: 64
- Other events: 0
- Date range: 2020-12-04 10:15:16+00:00 → 2026-09-08 21:42:36+00:00
- Unique track URIs: 20,393
- Unique artists: 9,164
- Exact duplicate observations: 134
- Core-event duplicate observations: 152

Duplicates are preserved as exported listening events; they are not silently discarded.
Sensitive fields `username`, `ip_addr_decrypted`, and `user_agent_decrypted` are excluded from the analytical database.
