# plugin-youtube

YouTube channel subscription and video feed management.

## Status

Labs (experimental).

## Description

Subscribes to YouTube channels and syncs videos into ECHO. Stores video metadata, transcripts, and thumbnails for analysis. Each channel exposes Sync and Clear actions; videos are rendered as articles and cards with transcript-aware companions.

## Features

- **Channel subscriptions**: Add a channel by URL, handle (@name), or channel ID.
- **Video sync**: Pull recent uploads (with optional restricted-mode cap).
- **Transcripts**: Fetch captions via `youtube-caption-extractor`.
- **Per-channel credentials**: Optional Google access token override.
- **Blueprint**: Exposes `Sync` and `ClearSyncedVideos` to the AI runtime.
- **Surfaces**: Channel article, channel properties, video article, video card.

## Schema

- `org.dxos.type.youtubeChannel` (`YouTubeChannel`)
- `org.dxos.type.youtubeVideo` (`YouTubeVideo`)
