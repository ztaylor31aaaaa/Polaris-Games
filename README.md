# Polaris Games

This repository is the community game catalogue for [Polaris](https://polaris.sdevs.workers.dev).

## Add a game

1. Create a folder inside `games/`, for example `games/my-game/`.
2. Put the game's entry page at `games/my-game/index.html`.
3. Add an `icon.svg` (or PNG) and optional `metadata.json`.
4. Add an entry to the root `catalogue.json`.

Example catalogue entry:

```json
{
  "id": "my-game",
  "name": "My Game",
  "description": "A short description.",
  "category": "Arcade",
  "src": "games/my-game/index.html",
  "image": "games/my-game/icon.svg"
}
```

Commit the changes to `main`. Polaris reads this catalogue from GitHub automatically; no change to the main Polaris repository is needed for each new game.

Games are displayed inside a sandboxed iframe. Keep each game's assets inside its own folder and use relative paths.

## Requirements

- Each game must have an `index.html` entry point.
- Use relative asset paths (for example `./style.css`).
- Keep catalogue IDs unique.
- Only add games you have permission to publish.
