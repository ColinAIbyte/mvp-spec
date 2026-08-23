# Idea → MVP Spec

Paste a product idea, get back a scoped MVP plan: the one core loop worth building
first, what to cut from v1, three milestones, and the risk most likely to sink it.

**Live:** https://colinaibyte.github.io/mvp-spec/

## How it works

A single static HTML file. No build step, no dependencies, no server.

You bring your own API key — it is kept in `localStorage` on your device and sent
only to the provider you pick (OpenAI or Anthropic). Nothing passes through a
backend, because there isn't one.

- Streaming responses, parsed from both providers' SSE formats
- Minimal Markdown renderer (headings, lists, bold) — no library
- Light and dark themes, mobile-first layout

## Why it exists

I build AI-powered MVPs for founders. This is a small, honest demonstration of
the thing I actually sell: taking a vague idea and cutting it down to something
you can ship in a week.

Built by Colin — https://colinaibyte.github.io/doudou-maze/en/

## Running locally

    python3 -m http.server 8901

Then open http://localhost:8901/
