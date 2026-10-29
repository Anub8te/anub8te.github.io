---
version: alpha
name: After Hours
description: A low-level security notebook with restrained anime scenery and colorful terminal typography.
colors:
  background: '#131521'
  surface: '#1b1d2b'
  raised: '#222638'
  text: '#e9e8ef'
  muted: '#a9abbf'
  faint: '#9496af'
  border: '#34374c'
  primary: '#c7adff'
  mint: '#97ddca'
  blue: '#91c7ff'
  peach: '#eca58e'
typography:
  display:
    fontFamily: 'Pixelify Sans, monospace'
  heading:
    fontFamily: 'Chakra Petch, Segoe UI, sans-serif'
  body:
    fontFamily: 'DM Sans, Segoe UI, sans-serif'
  utility:
    fontFamily: 'IBM Plex Mono, Consolas, monospace'
  japanese:
    fontFamily: 'Noto Sans JP, Yu Gothic, Meiryo, sans-serif'
rounded:
  sm: '6px'
  lg: '10px'
spacing:
  section: '64px'
  page: '1280px'
components:
  button: {}
  post: {}
  search: {}
  contents: {}
---

# Design notes

The site uses the After Hours visual system: dark surfaces, restrained accent colors, terminal-inspired components, anime scenery, local fonts, responsive spacing, and a theme switcher.

The homepage is a personal profile with a hero, a logbook of write-ups with topic filters, a research area, and a friends shelf. Search (press `/`), archives, and an RSS feed are available site-wide. Keep the visual language consistent when extending the site, and do not add placeholder achievements or unverified people.
