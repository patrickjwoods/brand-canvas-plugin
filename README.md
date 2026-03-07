# Brand Strategy Canvas — Claude Code Plugin

An interactive brand strategy coach for early-stage startup founders, built as a Claude Code plugin. Based on the book *[The Brand Strategy Canvas](https://www.amazon.com/Brand-Strategy-Canvas-One-Page-Startups/dp/148425158X)* by Patrick Woods.

## What It Does

This plugin guides founders through the 9-box Brand Strategy Canvas — a structured framework for building brand strategy *before* jumping to logos, taglines, and websites.

A single `/canvas` command routes intelligently based on your current state: starting fresh, picking up where you left off, or reviewing a completed canvas. When you're done, you'll have two files saved to your project directory:

- **`brand-canvas.md`** — the full strategic document
- **`brand-canvas.excalidraw`** — a visual layout of all 9 boxes; drag into [excalidraw.com](https://excalidraw.com) to see how everything fits together

## Installation

### From GitHub (recommended)

First, add this repo as a marketplace:

```bash
/plugin marketplace add patrickjwoods/brand-canvas-plugin
```

Then install the plugin:

```bash
/plugin install brand-canvas@patrickjwoods/brand-canvas-plugin
```

### For local testing

Clone the repo and point Claude Code at it directly:

```bash
git clone https://github.com/patrickjwoods/brand-canvas-plugin
claude --plugin-dir ./brand-canvas-plugin
```

## Usage

### Start or continue your canvas

```
/canvas
```

Auto-detects your current state and routes to the right section.

### Jump to a specific section

```
/canvas opportunity   # Market Opportunity (boxes A, B, C)
/canvas benefits      # Rational & Emotional Benefits
/canvas position      # Positioning Statement & Brand Essence
/canvas voice         # Values, Personality, Key Messages
```

### Start a new version

```
/canvas new
```

Archives your current canvas with a version stamp and starts fresh.

## The 9-Box Framework

The canvas moves through four sections in order:

| Section | Boxes | Description |
|---|---|---|
| **Market Opportunity** | Audience, Competition/Market, You | Who you're for, who you're against, what you do |
| **Benefits** | Rational, Emotional | What customers get — functionally and emotionally |
| **Positioning** | Statement + Essence | The single sentence that crystallizes your brand |
| **Voice & Expression** | Values, Personality, Key Messages | How you show up and what you consistently say |

Each section is coached interactively — the plugin asks questions, waits for your answers, and helps you synthesize before writing anything to the canvas.

## When to Use This

The framework is designed for founders at or approaching product-market fit. Pre-PMF, the plugin will flag this and recommend a lighter-weight path.

## About

Created by [Patrick Woods](https://patrickwoods.com). Questions or feedback: [@patrickjwoods](https://twitter.com/patrickjwoods).

Learn more about the framework at [thebrandstrategycanvas.com](https://thebrandstrategycanvas.com) or pick up the book: *[The Brand Strategy Canvas](https://www.amazon.com/Brand-Strategy-Canvas-One-Page-Startups/dp/148425158X)* (Apress).
