# Visual Diff for Claude Code Web

**Demo:** [Live Prototype](https://ccgrowth.vercel.app/demos/visual-diff/)

## What This Shows

A UX prototype demonstrating inline visual diffs in Claude Code Web — showing before/after screenshots of UI changes directly in the chat, without leaving the conversation.

## The Problem

Developers working on UI are "coding blind" in Claude Code Web:

Code → Commit → Deploy → Open preview → Check result → Context switch back

## The Solution

Automatically capture and display visual diffs inline:

- Detect deployment preview URLs (Vercel, Netlify, etc.)
- Screenshot before (production) and after (preview)
- Show side-by-side comparison in chat
- Auto-populate PR descriptions with visual changes

## Making This Real

This is a static prototype. A real implementation needs:

1. **Screenshot service** — Playwright/Puppeteer or hosted API
2. **Deployment platform integrations** — Auto-detect preview URLs
3. **MCP Server** — For Claude Code/Cursor integration

## Inspiration

[vercel-labs/before-and-after](https://github.com/vercel-labs/before-and-after) — CLI tool that proves the concept. This prototype shows how it could work natively in Claude Code Web.
