# GlassTerm

A first-generation Google Glass Explorer Edition repurposed as a persistent, voice-driven Claude Code terminal.

The project page lives in `index.html` and is intentionally zero-dependency: plain HTML and CSS, no framework, no build step, no JavaScript.

## GitHub Pages

Publish from:

- Branch: `main`
- Folder: `/ (root)`

Expected URL:

https://voidnullvalue.github.io/glassterm/

## Architecture

```text
Google Glass
   | \
   |  \ microphone audio
 SSH   \
   |    v
   |  fenchurch
   |  whisper.cpp
   |    |
   |    | transcription
   v    v
development workstation
   |
   v
tmux: glass
   |
   v
Claude Code
```
