# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

A minimal, static "under construction / coming soon" landing page. Single `index.html` with embedded CSS and JS — no build step, no dependencies.

## Deployment

The site is deployed on **Vercel** as a static site. Pushing to the main branch triggers an automatic redeploy.

- Live URL is set in the Vercel project dashboard.
- No `vercel.json` is needed; Vercel auto-detects a static site from `index.html`.

## Design Principles

- Dark background (`#0a0a0a`), muted palette, no color accent beyond the green pulse dot.
- All styles are inline in `index.html` using CSS custom properties defined in `:root`.
- Typography uses the system font stack — no external font imports.
- Responsive via `clamp()` and relative units only.

## Editing

To change the headline, description, or email CTA, edit the relevant HTML in `index.html`. The color palette is controlled entirely by the `:root` variables at the top of the `<style>` block.
