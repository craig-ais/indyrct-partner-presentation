# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a self-contained HTML slide presentation for the "Cotillion Platform" - a trust infrastructure platform for the technology channel (TSPs/MSPs). The presentation is designed to recruit Proof of Concept partners.

## Architecture

The entire presentation lives in a single HTML file (`Services Partners cotillion_presentation.html`) containing:
- **CSS**: Custom styling with CSS variables for theming (purple color palette), responsive grid layouts, and slide transitions
- **JavaScript**: `PresentationController` class handling keyboard navigation, chapter navigation, progress tracking, and slide transitions
- **Assets**: SVG logos embedded inline; external images (PNG/JPG/SVG) in the same directory

## Key Technical Details

- **Color scheme**: Uses CSS custom properties (`--primary-purple: #73026B`, `--accent-purple: #a5039a`, `--dark-purple: #41013c`)
- **Navigation**: Arrow keys for slide navigation, clickable sidebar chapters, Home/End keys for first/last slide
- **Slide system**: Slides use `data-chapter` attributes for chapter grouping; active slide controlled via `.active` class
- **Responsive**: Media query at 1200px breakpoint adjusts grid layouts and typography

## Development

Open `Services Partners cotillion_presentation.html` directly in a browser - no build process or server required.

## Brand Assets

Logo files follow naming convention: `[Orientation] [Color] logo - [background].svg`
- Orientations: Standard, Vertical
- Colors: Black, White, Color
- Backgrounds: "no background", "with background"
