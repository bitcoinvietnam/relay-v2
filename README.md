# BV Relay

Landing page for [BitcoinVN's Nostr Relay](https://nostr.bitcoinvn.io) service.

## Tech Stack

- [Eleventy (11ty)](https://www.11ty.dev/) v3 - static site generator
- [Nunjucks](https://mozilla.github.io/nunjucks/) - templating
- Native CSS with custom properties
- No frameworks or build tools beyond Eleventy

## Getting Started

```bash
pnpm install
pnpm run dev
```

The site will be available at `http://localhost:8080`.

## Build

```bash
pnpm run build
```

Output goes to `_site/`.

## Project Structure

```
src/
├── _includes/
│   ├── base.njk          # HTML shell, scripts
│   ├── header.njk        # Sticky navbar
│   └── footer.njk        # Footer with social links
├── _data/
│   ├── site.json         # Site metadata, nav links
│   ├── sections.json     # Homepage content data
│   └── specs.json        # Relay hardware specs
├── css/
│   └── style.css         # All styles
├── assets/
│   ├── blue-spark.webp   # Hero background
│   └── bvn-star.svg      # Brand logo
├── index.njk             # Homepage
├── specs.njk             # Relay specifications
└── tos.njk               # Terms of Service
```

## Pages

- **Home** - Hero, about Nostr, why paid relays, why BV Relay, member benefits, join CTA
- **Specs** - Relay hardware specifications and WSS address
- **TOS** - Terms of Service

## License

Proprietary - BitcoinVN.
