# Dev Portfolio — Pixel Edition

> Retro pixel/arcade-style developer portfolio of Rahmatul Usra (@xsrazy): 16 live projects, top starred repos, and a skill tree, all framed like a game character profile screen.

[![Live](https://img.shields.io/badge/live-dev.xsrazy.web.id-brightgreen)](https://dev.xsrazy.web.id)

**Live site: https://dev.xsrazy.web.id**

## About

A single-page portfolio styled like a retro game: pixel fonts, chunky 4px pixel-panel borders, a scanlines overlay, and pixelated images. The header is a "player card" with the author's GitHub avatar, a bio line, live GitHub stats, a blinking PRESS START anchor, and a CONTACT side panel. Below it sit the live projects grid, a Top Loot section of the most-starred repos, a swipeable strip of more repos, and a Skill Tree of languages by repo count. The GitHub sections load live data from the GitHub API and fall back to baked-in snapshot data when the API is unreachable.

## Player Card

- **Avatar and name:** GitHub avatar (pixelated rendering) with the name RAHMATUL USRA (@XSRAZY).
- **Bio:** "i don't need school, i have google!" from Sumatera Barat, Indonesia.
- **Live stats:** years on GitHub, public repo count, followers, and total stars, fetched from the GitHub API.
- **PRESS START:** a blinking anchor that jumps to the projects section.
- **CONTACT panel:** buttons for GitHub and email, plus a 16 live projects stat.

## Projects

| Project | Category | Description |
|---|---|---|
| [NikahPee](https://nikahpee.xsrazy.web.id) | Wedding invitations | Shopee-style wedding invitation for Usra & Zee. |
| [NikahTube](https://nikahtube.xsrazy.web.id) | Wedding invitations | YouTube-style wedding invitation, free and open source. |
| [Wedify](https://wedify.xsrazy.web.id) | Wedding invitations | Spotify-style wedding invitation, free and open source. |
| [samaWA](https://samawa.xsrazy.web.id) | Wedding invitations | WhatsApp-style wedding invitation for Usra & Zee. |
| [Nikah](https://nikah.xsrazy.web.id) | Wedding invitations | Classic digital wedding invitation for Usra & Zee. |
| [NikahFix](https://nikahfix.xsrazy.web.id) | Wedding invitations | Netflix-style wedding invitation. |
| [LinkPass](https://linkpass.xsrazy.web.id) | Web tools and apps | Free open-source link-in-bio generator with a digital pass concept. |
| [TikBulk](https://tikbulk.xsrazy.web.id) | Web tools and apps | Bulk TikTok video downloader, no watermark. |
| [Tools](https://tools.xsrazy.web.id) | Web tools and apps | 1,108 free micro tools that run entirely in the browser. |
| [CekTag](https://cektag.xsrazy.web.id) | Web tools and apps | GetContact tag checker for unknown numbers. |
| [TMail](https://tmail.xsrazy.web.id) | Temp mail | Free temporary email, no sign-up, auto-deletes in 24 hours. |
| [myrobs.store](https://myrobs.store) | Store and catalog | Roblox services store. |
| [FMCreators Marketplace](https://fmc.xsrazy.web.id) | Store and catalog | Curated Roblox clothing catalog. |
| [Masakan Kekinian](https://msknkkn.xsrazy.web.id) | Recipes | Recipe discovery site. |
| [GitHub Readme Stats](https://github-readme-stats.xsrazy.web.id) | Developer | Self-hosted GitHub profile card suite: graph, stats, streak, languages, trophy. |
| [ShareCanva](https://sharecanva.com) | Design | Free monthly Canva Pro invite links. |

## Features

- **Pixel/arcade theme.** Press Start 2P and VT323 fonts from Google Fonts, a dark navy palette, 4px black pixel-panel borders with inset shading, a fixed scanlines overlay, and pixelated image rendering.
- **Category filter.** Filter chips for All and each project category, filtering the grid in place.
- **In-page preview modal.** Every project card has a PREVIEW button that opens a floating window with the project's live site inside an iframe. The modal bar shows the project name, an OPEN TAB link, and a CLOSE button. It also closes on Escape or backdrop click, locks page scrolling while open, and clears the iframe on close.
- **VISIT buttons.** Every card has a VISIT button that opens the project in a new tab.
- **Top Loot.** The 10 most-starred repos, loaded live from the GitHub API (sorted by stars), each with its language color dot and star count.
- **More Repos swipe strip.** A horizontal scroll-snap strip of further repos: non-fork repos with a homepage, excluding the top 10, also loaded live from the GitHub API.
- **Skill Tree.** Language bars showing repo counts per language, computed live from the GitHub API and scaled to the top language.
- **Static fallback data.** Every GitHub-powered section ships with baked-in snapshot data, so the page still renders fully if the GitHub API request fails or is rate-limited.
- **Responsive.** Below 560px the header grid stacks (smaller avatar, bio and stats full-width, contact panel unboxed) and card gaps tighten.

## Architecture

- **Frontend:** a single static `index.html` file with vanilla HTML, CSS, and JavaScript. No build step, no framework, no dependencies beyond Google Fonts.
- **Backend:** none. No server code and no database. Live GitHub data is fetched client-side from the public GitHub REST API (user profile plus up to 100 repos, sorted by stars, unauthenticated).
- **Hosting:** Vercel project `dev-portfolio-pixel`, at [dev.xsrazy.web.id](https://dev.xsrazy.web.id).

## Files

- `index.html`: the entire portfolio page (markup, pixel styles, project data, filter, preview modal, GitHub sections).
- `thumbs/`: custom project screenshots referenced by the project cards (14 projects; Masakan Kekinian and ShareCanva use live snapshot images instead).

## Credits

Built by [Rahmatul Usra (@xsrazy)](https://github.com/xsrazy). Project and repo data from [github.com/xsrazy](https://github.com/xsrazy).

## License

No license is specified for this version.
