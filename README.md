# ILC.CloudPages.DevTools

Interactive developer tools for [fb.js](https://github.com/ilc-global/ILC.Fishbowl.JS) and fishbowl.js. Each page is a working diagnostic/testing tool — not a static demo.

## Pages

| # | Page | Purpose |
|---|------|---------|
| 00 | [Environment & Context](00_Environment.html) | Runtime detection, user context, available methods, access rights, logging |
| 01 | [SQL Console](01_SQL_Console.html) | Parameterized SQL runner with DataTables results |
| 02 | [Legacy API Explorer](02_Legacy_API_Explorer.html) | Browse all 109 API calls, build requests, view normalized responses |
| 03 | [REST API Tester](03_REST_API_Tester.html) | Method/path/body form with history |
| 04 | [CSV Import Builder](04_CSV_Import_Builder.html) | Explore 56 import types, build CSV from JSON, execute imports |
| 05 | [Reports & Printing](05_Reports_Printing.html) | Report preview/PDF, printer listing, PDF/ZPL printing |
| 06 | [Navigation & UI](06_Navigation_Dialogs.html) | Module hyperlinks, status bar, progress, fullscreen, scheduled tasks |
| 07 | [Files & Plugin Data](07_Files_PluginData.html) | Read/save files, plugin data CRUD |
| 08 | [Timezone](08_Timezone.html) | Server/client time conversion, multi-timezone comparison |

## Setup

Copy `fb.js` and `fishbowl.js` into the `js/` directory:

```
ILC.CloudPages.DevTools/
├── js/
│   ├── fb.js           # from ILC.Fishbowl.JS
│   └── fishbowl.js     # from ILC.Fishbowl.JS
├── sql/
│   └── 03_Query.sql    # sample SQL file for SQL Console
├── 00_Environment.html
├── 01_SQL_Console.html
├── ...
└── 08_Timezone.html
```

To use in Fishbowl, copy the HTML files and `js/` folder into your CloudPages plugin directory.

## Dependencies

| Library | Loaded via | Used by |
|---------|-----------|---------|
| [fb.js](https://github.com/ilc-global/ILC.Fishbowl.JS) | Local (`js/fb.js`) | All pages |
| [fishbowl.js](https://github.com/ilc-global/ILC.Fishbowl.JS) | Local (`js/fishbowl.js`) | 02 Legacy API, 04 CSV Import |
| Bootstrap 5.3 | CDN | All pages |
| jQuery 3.7 | CDN | 01 SQL Console |
| DataTables 1.13 | CDN | 01 SQL Console |

## License

ILC Technology LLC Source-Available License v1.0 — see [LICENSE](LICENSE).
