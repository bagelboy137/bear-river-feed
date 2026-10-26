# Bear River report feed

`reports.json` is the fishing-report feed for Bear River, a personal iPhone app for anglers and
paddlers. For each of 41 streams in Pennsylvania, New York and Maryland it has what local fly shops
said in their latest reports: a condition, a summary of 25 words or fewer written in our own words,
the hatches and flies they mention, and a link to the shop's own report. Read the shop's page for
the full report.

- **The shops' words stay theirs.** No shop text is copied here. Each summary is checked against
  the shop's page and rejected if it repeats eight or more words in a row.
- **Each report keeps the date the shop wrote it.** The feed is gathered about twice a day, but the
  reports are only as new as the shops make them.
- **Polite reading.** The gatherer reads only the shop pages listed as readable, identifies itself
  as `BearRiverReportBot`, honors robots.txt and crawl delays, and stops at any block. Shops whose
  terms don't allow automated reading appear only as links (`links` on each stream); nothing reads
  them.

**Shop owners:** if you'd like your shop's reports left out, or summarized differently, open an
issue here and it will be done on the next run.

Schema version 1: `generatedAt`; `sources` (shop, page, last checked); `streams` (river, state, USGS
gauge ids, `reports`, `links`).

`osm/` holds OpenStreetMap state packs (river launches, parking, campsites, dams) that the app downloads per
state, © OpenStreetMap contributors under the ODbL; see `osm/README.md`.
