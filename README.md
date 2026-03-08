# pochapochi

`pochapochi` is a static, end-to-end encrypted peer-to-peer chat app extracted from the Battlegrid codebase.

The app is intentionally chat-only in this repository. The original Ollama/local-AI code is still present in `index.html`, but it is hard-disabled behind `AI_FEATURE_ENABLED = false` so the UI and automatic reply logic stay off.

## Files

- `index.html` contains the working app.
- `app.js` and `styles.css` are preserved placeholders from the source snapshot.

## How to use

Open `index.html` in a browser or deploy the folder as a static site. The first visitor to a room URL becomes the room creator, and the invite link includes the encryption key in the `#k=` fragment.

## Notes

- Messages are synchronized through GunDB relays.
- Only people with the full invite link can decrypt chat messages.
- This repo intentionally excludes the stale Battle Grid spec and internal architecture docs from the original app snapshot.
