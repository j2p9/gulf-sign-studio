# Licensed official sign fonts

Put your licensed font files here (TTF or OTF — WOFF2 is not supported by the shaping engine):

| Role | Official typeface | Used for |
|---|---|---|
| `latinHeavy` | Transport Heavy | English text on light backgrounds (SHC 602 §3.1.3.6) |
| `latinMedium` | Transport Medium | English text on dark backgrounds |
| `arabic` | Boutros Advertisers Naskh | Arabic text (Naskh, required by SHC 602 and the Abu Dhabi MUTCD) |

Then copy `fonts.example.json` to `fonts.json` and edit the file names to match yours.
Reload the site — the top bar changes from "Stand-in fonts" to "Official fonts".

**Licensing:** a public website sends these files to every visitor's browser, so your licence
must allow web/app embedding. The files in this folder are git-ignored and never committed, and
`npm run deploy` refuses to publish them unless you set `ALLOW_LICENSED_FONTS=1`.
Exported PDFs, SVGs, DXFs and 3D models contain outlines only, not the font files.
