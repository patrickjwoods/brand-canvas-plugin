# Brand Strategy Canvas — Claude Code Plugin

An interactive brand strategy coach for early-stage startup founders, built as a Claude Code plugin. Based on the book *The Brand Strategy Canvas* by Patrick Woods (Apress).

## What It Does

This plugin guides founders through the 9-box Brand Strategy Canvas — a structured framework for building brand strategy *before* jumping to logos, taglines, and websites.

A single `/canvas` command routes intelligently based on your current state: starting fresh, picking up where you left off, or reviewing a completed canvas. All work is saved to a `brand-canvas.md` file in your project directory.

## Installation

```bash
claude plugin install brand-canvas
```

Or directly from GitHub:

```bash
claude plugin install github:patrickwoods/brand-canvas-plugin
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
| **Market Opportunity** | A, B, C | Who you're for, who you're against, what you do |
| **Benefits** | Rational, Emotional | What customers get — functionally and emotionally |
| **Positioning** | Statement + Essence | The single sentence that crystallizes your brand |
| **Voice & Expression** | Values, Personality, Key Messages | How you show up and what you consistently say |

Each section is coached interactively — the plugin asks questions, waits for your answers, and helps you synthesize before writing anything to the canvas.

## Output

Work is saved incrementally to `brand-canvas.md` in your current directory. You can open, edit, and share this file directly.

## When to Use This

The framework is designed for founders at or approaching product-market fit. Pre-PMF, the plugin will flag this and recommend a lighter-weight path.

## About the Book

*[The Brand Strategy Canvas](https://www.amazon.com/Brand-Strategy-Canvas-One-Page-Startups/dp/148425158X)* by [Patrick Woods](https://patrickwoods.com) teaches early-stage founders how to do strategic brand thinking before execution. Available from Apress.
