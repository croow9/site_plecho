# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static single-page landing page for "Плечом к плечу" (Shoulder to Shoulder) — a mobile app that helps users find workout partners. Built with plain HTML/CSS/JS (no frameworks, no build tools).

- **Language**: Russian (all UI text is in Russian)
- **Created with**: [Omma](https://omma.build)

## Running Locally

Open `index.html` directly in a browser, or serve it:

```bash
npx serve .
```

No build step, no dependencies to install.

## Architecture

Everything lives in a single `index.html` file (~1850 lines):
- **CSS** is embedded in a `<style>` block (lines ~8–1400) using CSS custom properties defined in `:root`
- **HTML** sections: nav, hero, stats, features, social proof, download CTA, footer
- **JavaScript** is embedded in a `<script>` block at the end, handling: scroll-based nav styling, mobile menu toggle, IntersectionObserver animations, animated counters, parallax effects, smooth anchor scrolling

## Key Design Tokens (CSS Variables)

`--navy`, `--deep-blue`, `--electric`, `--bright-blue`, `--azure`, `--light-azure`, `--glow` — the blue-themed color palette. `--glass-bg` and `--glass-border` for glassmorphism effects.

## Assets

- `1.jpg`–`6.jpg` (also duplicated in `assets/`): screenshot/promo images used in hero background and feature cards
- `brjy.png`: logo image
- `promt.txt`: Russian-language change request notes (not part of the site)
