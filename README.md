# Simlas Documentation

Public documentation for **Simlas**, a Discord companion for *The Witcher TRPG*.

Simlas is currently in active development and is being tested with invited users. This repository contains public, player-facing documentation only. The application source code, internal architecture documents, private source material, and development records remain private.

## Start here

- [Player Guide](docs/PLAYER_GUIDE.md) — how to join a game, use your character, take turns, attack, defend, manage equipment, and troubleshoot common situations.
- [Tester Guide](docs/TESTER_GUIDE.md) — how to test Simlas during development and how to report unexpected behavior usefully.

## Documentation site

The [`docs/`](docs/) directory is intentionally structured so this repository can later become the public Simlas documentation website through GitHub Pages.

For now, the Markdown files in this repository are the canonical public documentation.

## Development status

Simlas is not yet a public hosted service.

Commands, workflows, and behavior may change while testing continues. If this documentation and the currently running bot disagree, use `/help` in Discord to check the command surface available on that bot instance and report the mismatch.

## Reporting issues

If Simlas behaves unexpectedly during testing:

1. Do not repeatedly retry a command unless Simlas explicitly tells you to.
2. Record the command you used.
3. Copy the full Simlas response.
4. Include what you expected to happen.
5. Include what happened instead.
6. Tell the GM or test coordinator whether the issue happened before or after restarting Simlas.

See the [Tester Guide](docs/TESTER_GUIDE.md) for more detail.

## Disclaimer

Simlas is an unofficial fan-made companion project for *The Witcher TRPG*.

It is not affiliated with or endorsed by CD PROJEKT RED, R. Talsorian Games, or the owners of *The Witcher* intellectual property.

This documentation does not reproduce game books or private source material.
