# 🎵 Mēles — Reed Log

Bassoon reed logging web app. Logs reeds as Markdown notes straight into an Obsidian vault via GitHub.

**Live app:** https://meisswindu.github.io/reed-log/

## What it does
- **Jauna mēle** — register a reed (auto ID: L=Lavoro, D=Danzi, R=Rigotti, NZ=Normunds)
- **Ātrais log** — pick a reed, tap a 1–10 rating, optional note → saved with timestamp
- **Bibliotēka** — rating history, sparklines, similar-reed matching
- Writes notes in the exact vault format (frontmatter + Mērījumi/Testēšana/Piezīmes/Log sections)

## Setup
1. Create a fine-grained GitHub personal access token (Settings → Developer settings), scoped to your vault repo only, **Contents: Read and write**
2. Paste it in the app's ⚙️ card
3. Press "⬇️ Ielādēt mēles no GitHub"

## Tech
Single self-contained HTML file, no build step, no dependencies. Data syncs to the Obsidian vault repo via the GitHub Contents API.
