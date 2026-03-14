# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Single-file browser game (`tictactoe.html`) — no build step, no dependencies, no package manager.

## Development

Open `tictactoe.html` directly in a browser to run the game. There are no build, lint, or test commands.

## Architecture

Everything lives in `tictactoe.html`: inline CSS in `<style>`, markup in `<body>`, and vanilla JS in `<script>`.

- **Board state** — a flat 9-element array (`board[]`), indexed 0–8 left-to-right, top-to-bottom.
- **Win detection** — checked after every move against the 8 `WINS` combinations; returns the winning line indices for highlight animation.
- **Score** — persists across restarts in a plain `scores` object (`X`, `O`, `D`); reset only on page reload.

## Git & GitHub

- Remote: `git@github.com:Loup-Noe/tic-tac-toe.git`
- Branch: `master`
- Commit and push after every meaningful change.
