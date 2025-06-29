# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for Ann Leahy, an ICF-certified executive coach. The project consists of a single HTML file with embedded CSS and JavaScript, creating a responsive professional coaching website.

## Architecture

### Single-Page Application Structure
- **Main file**: `ann_leahy_menu.html` - Complete website in one HTML file
- **Embedded styling**: CSS is contained within `<style>` tags in the HTML head
- **Embedded JavaScript**: Minimal JavaScript for mobile menu functionality
- **Static assets**: Images (headshot.jpg, beach.png, acc.png, brand.png) for visual content

### Key Components
- **Navigation**: Sticky header with responsive hamburger menu for mobile
- **Hero Section**: Beach image with overlay navigation
- **About Section**: Professional headshot and bio content
- **Approach Section**: Three-step coaching methodology display
- **Contact Section**: Contact form (non-functional, frontend only)
- **Footer**: Professional credentials display

### Styling Architecture
- **Typography**: Uses Google Fonts (Prata for headings, Work Sans for body)
- **Color Scheme**: 
  - Primary: #0f2e33 (dark teal)
  - Secondary: #5b8296 (blue-gray)
  - Accent: #b47979 (rose)
  - Background: #f8f8f8 (light gray)
- **Responsive Design**: Mobile-first approach with breakpoint at 768px

## Development Notes

### File Structure
- No build process or package management
- Direct file editing for content updates
- Images should be optimized for web before adding
- Single HTML file makes deployment simple

### Making Changes
- All styling changes go in the `<style>` section (lines 9-218)
- Content updates are made directly in HTML body
- Mobile menu functionality is in the `<script>` section (lines 288-293)
- Navigation links use anchor tags pointing to section IDs

### Browser Compatibility
- Uses modern CSS features (flexbox, sticky positioning)
- Responsive design implemented with CSS media queries
- JavaScript is minimal and broadly compatible