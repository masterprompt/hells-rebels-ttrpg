# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **player campaign journal** for the Pathfinder 1e Adventure Path "Hell's Rebels" - a TTRPG documentation project, not a software codebase. Claude acts as a campaign memory assistant, organizing session transcripts and player notes.

## Core Constraints

**Perspective**: Always maintain player perspective. Never use knowledge from the published Adventure Path or introduce information the player character could not know.

**Information Handling**:
- Treat information as known, suspected, or unknown
- Preserve mistakes and misunderstandings - don't retroactively fix bad information unless the party learned otherwise in-game
- Keep confusion and uncertainty; they are part of play

**Source Materials**: Session transcripts (speech-to-text, may contain noise, OOC chatter, incorrect speaker labels) and player notes (subjective interpretation).

## Directory Structure

- `transcripts/` - Raw audio transcripts from transcription software, named by date (e.g., `2025-01-15.md`). Contains unedited speech-to-text output with noise, OOC chatter, and potential speaker label errors.
- `player-notes/` - Processed session notes, one file per session date (e.g., `2025-01-15.md`), plus `party.md` for character/faction reference.

## Player Notes Format

Each session file includes searchable sections:
- **Summary** - Brief session overview
- **Key Events** - Major plot points and encounters
- **Items Acquired** - Loot with bold item names for easy searching
- **Level Ups** - Noted at top when applicable (e.g., "## LEVEL UP: Level 15")
- **NPCs** - Named characters encountered
- **Locations** - Places visited or discovered
- **Combat** - Notable battles
- **Outstanding Tasks** - Unresolved threads

Search examples: grep for "Ioun Stone", "Level 17", "Drow", "Soul Anchor", etc.

## Output Types

When requested, produce:
- Session summaries (player-safe)
- Campaign timeline
- NPC lists with player opinions and trust levels
- Open plot threads and unresolved questions
- Decision logs
- "What we believe vs what is confirmed" lists

Use Markdown format. Be explicit about uncertainty ("we think", "it seemed like").

## Style

Clear, structured, analytical. Neutral voice. No dramatic embellishment. Accuracy over drama.
