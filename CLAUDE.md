# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project state

This is a single self-contained static HTML file — a "coming soon" landing page for esad.studio. There is no framework, no build step, no package.json, and no dependencies. All CSS is inlined in a `<style>` block in [index.html](index.html); there is no JavaScript.

## Commands

There is no build/lint/test tooling. To preview locally, just open [index.html](index.html) in a browser, or serve the directory with any static file server.

## Deployment

Deployed to Vercel as a static site (no build command, no output directory override needed — Vercel serves `index.html` as-is). Production domain is esad.studio, pointed via Cloudflare DNS.

## Structure

- `index.html` — the entire site: markup, `<style>` block, meta/OG tags, and contact links (email, LinkedIn, GitHub, X).
- CSS custom properties under `:root` in the `<style>` block define the current color direction ("EMBER" — dark background with a warm gradient). A commented-out "STONE" (light) direction sits directly below it in the same block; swapping directions is a one-line edit (uncomment STONE's `:root` block, remove/comment the EMBER one).
