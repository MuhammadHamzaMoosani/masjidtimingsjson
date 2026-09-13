# masjid-timings-board

Public data feed for the [Jamaat Reader](https://github.com/MuhammadHamzaMoosani/masjidTimings) app.

Holds nothing but the daily board: `timings.json` (fetched by the app at runtime via
`NEXT_PUBLIC_BOARD_URL`) and the board photos it was read from, one per date, in
`images/`. Updated by `ingest/update.py` in the main app repo — never hand-edited here.

No app code, no ingestion scripts, no WhatsApp automation. That stays in the private
repo; this one only exists so the app can pick up a new board without a rebuild.
