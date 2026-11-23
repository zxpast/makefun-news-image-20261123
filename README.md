# The World in One Page — Monday 23 November 2026

[![make.fun](https://img.shields.io/badge/make.fun-news--image--20261123-red)](https://make.fun/c/news-image-20261123)
[![Node](https://img.shields.io/badge/node-22-green)](https://nodejs.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A make.fun entry for **news-image-20261123**: sum up Monday 23 November 2026's
world news in one image.

`main.ts` (Node 22, standard library only, no network) draws a broadsheet front
page — masthead date, kicker, stat strip, region strip, three hero cards with
drawn scenes, ten illustrated cards, a world map with numbered pins, a numbered
brief list, and a DATE CHECK box — and writes a deterministic 1024×1024 PNG to
`/output/entry.png`. The program runs twice and writes byte-identical output.

37 stories, 6 regions, every story happened or was first reported on Monday
23 November 2026. Stories that broke on another day are listed in the DATE CHECK
box, not on the page.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## License

MIT — see [LICENSE](LICENSE).
