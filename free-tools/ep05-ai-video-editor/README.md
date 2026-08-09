# AI Video Editor — User Guide

Clean up a rough talking-head video in minutes — you approve every cut before anything is edited.

## Install

1. Download **EP05 AI Video Editor** from [Project A3 on GitHub](https://github.com/AlvinChiew/project-a3).
2. Run the installer and open **AI Video Editor**.

## Activate (one time)

1. On the welcome screen, read and tick the **disclaimer**.
2. Get a free activation code at [project-a3.alvinchiew.com](https://project-a3.alvinchiew.com/#signup).
3. Enter your code and business email, then click **Activate**.

## First-time setup

1. Open **Settings**.
2. Click **Set up video engine** to download FFmpeg (one-time, ~100 MB).
3. Paste your **OpenAI API key** and click **Save**, then **Test connection**.
   - Whisper charges your OpenAI account (~$0.006 per minute of audio).

## Edit a video (5 steps)

### 1 — Transcribe

- Click **New project** on the home screen and choose an MP4 or MOV file.
- Click **Transcribe** to generate a timestamped transcript from the actual audio.

### 2 — Process

- Red badges = suggested cuts (repeats, restarts). Yellow = review only (pauses, fillers).
- **Conservative** mode (default) preselects only high-confidence repeats — never a full sentence silently.
- Toggle **Cut** / **Keep** on each suggestion; use **Preview** to hear that section.
- Click **Continue to Frame** when done.

### 3 — Frame

- Drag the yellow crop box so the person fills the vertical frame — no black bars.
- Use **Keep full person visible** if needed, then **Save crop**.

### 4 — Subtitle

- Subtitles are timed from the **final** cut, not the original recording.
- Edit wording and line breaks, then **Continue to export**.

### 5 — Export

- Tick the QC checklist, choose a folder, and click **Export**.
- You get: final MP4, SRT, styled ASS, and project JSON.

## Tips

- Record in a quiet room — fewer false “cut” suggestions.
- If a natural pause sounds intentional, leave it on **Keep**.
- Reopen a project from the home screen to adjust cuts before exporting again.

## Common issues

| Problem | What to do |
| ------- | ---------- |
| “Set up the video engine” | Settings → download FFmpeg |
| “OpenAI API key is not configured” | Settings → paste key → Save |
| Transcription fails | Check internet, key balance, and file length |
| Subtitles drift | Re-export after changing cuts (timing is recalculated automatically) |

## Help

- [Project A3 website](https://project-a3.alvinchiew.com)
- Business inquiries: contact.project.a3@alvinchiew.com

Made Simple, For Business · Project A3
