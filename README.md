# Strapi Converter

Convert formatted content from Google Docs or HTML into Strapi-friendly Markdown.

## Overview

This tool streamlines the process of converting rich content from Google Docs or HTML directly into Markdown format optimized for Strapi CMS. Styled HTML callouts are intelligently converted to the closest Markdown equivalent—whether that's blockquotes, tables, or horizontal rules.

## Features

- **Dual Input Modes**
  - Paste directly from Google Docs
  - Paste HTML source code

- **Smart Callout Conversion**
  - Auto-detects styled blocks (backgrounds, borders, padding)
  - Converts to blockquotes, tables, horizontal rules, or plain content
  - Preserves label-value patterns as formatted tables

- **Live Preview**
  - Real-time Markdown preview
  - Side-by-side comparison with original

- **Content Intelligence**
  - Automatic word count, image detection, table and callout counting
  - Visual alerts for styling that cannot be preserved
  - Image upload reminders for manual re-upload to Strapi

- **One-Click Copy**
  - Copy converted Markdown directly to clipboard
  - Perfect for pasting into Strapi's rich text editor

## How to Use

1. Choose your input source: Google Docs paste or HTML source
2. Paste your content into the left pane
3. Select preferred callout style (if using HTML mode)
4. Copy the Markdown output from the right pane
5. Paste into Strapi

## Callout Styles

- **Auto**: Intelligently picks tables for label-value content, blockquotes for others
- **Blockquote**: Vertical bar callout style
- **Table**: Best for structured label-value lists
- **Horizontal Rules**: Dividers above and below content
- **None**: Removes styling, keeps plain content

## Technical Stack

- Vanilla JavaScript
- [Turndown](https://github.com/mixmark-io/turndown) for HTML-to-Markdown conversion
- [Turndown GFM Plugin](https://github.com/mixmark-io/turndown-plugin-gfm) for GitHub Flavored Markdown support

## Try It

Open `paste-helper-v3_1.html` in any modern browser to start converting content right away.
