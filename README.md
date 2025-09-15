# PinkSync Mesh Accessibility Starter

## Features

- Supabase schema for accessibility, sign language, captions, signals, assets, feedback
- FastAPI backend for accessibility endpoints (ready for Supabase integration)
- React hook example for live accessibility signals (with Supabase Realtime)
- Extendable for sign language models, gesture icons, visual overlays

## Quickstart

1. Deploy Supabase project and run `schema.sql`
2. Deploy FastAPI backend (`api/pinksync_accessibility.py`)
3. Use React/Next.js frontend; connect via hooks (`src/hooks/useAccessibilitySignals.js`)
4. Extend with sign language models, caption generation, and more!

## Table Design

- `profiles`: User accessibility preference (deaf, sign language, etc.)
- `signals`: WebRTC events with accessibility metadata
- `messages`: Chat/video with caption/sign flags
- `assets`: Sign video, captions, icons
- `feedback`: User feedback on accessibility experience

## Example Queries

- `/api/v1/accessibility/users?type=sign_language`
- `/api/v1/accessibility/messages?room_id=xyz&captioned=true`
- `/api/v1/accessibility/assets?type=sign_video`

## Extend

- Add ML models for sign recognition
- Enhance accessibility feedback, dashboards
- Integrate with PinkFlow and other PinkSync tools
