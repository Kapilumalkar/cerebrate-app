# Cerebrate — Claude Code Context

## What This Repository Is
Cerebrate is a systematic market intelligence platform.
This repository (cerebrate-app) is the LIVE POC — it runs
daily at 9:45 AM EST generating real predictions that form
the verified track record. It must never be broken.

## CRITICAL RULES
1. NEVER push directly to main branch
2. NEVER change the core analysis prompt without explicit instruction
3. NEVER modify the portfolio simulation logic without explicit instruction
4. ALWAYS create a new branch for every change
5. ALWAYS produce complete files — never partial code snippets

## Architecture
- Frontend: Single HTML file (index.html) hosted on GitHub Pages
- Proxy: Cloudflare Worker — handles Anthropic API, GNews, Yahoo Finance
- No build process — pure HTML/CSS/JS
- No frameworks — vanilla JavaScript only

## Design System
- Background: #03050D
- Gold accent: #C9A84C
- Emerald positive: #30C99A
- Coral negative: #E85555
- Body text minimum: #E8ECFF
- Fonts: Syne (UI), Cormorant Garamond (headings), JetBrains Mono (data)

## Framework Rules
- Signal threshold: 65% probability minimum to trade
- Never trade TIER3 source signals
- Never trade Kelly < 3%
- Never use VIX as instrument (use VIXY instead)
- No duplicate tickers in portfolio
- Max 15% per instrument, 40% per sector, 60% deployed
- Half-Kelly sizing always

## Current Status
Live POC running — handle with extreme care
