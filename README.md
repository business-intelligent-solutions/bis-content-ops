# bis-content-ops

Shared SEO content assets for BIS and vShopper's content-generation skills. Public repo by design — every file here is fetchable with plain, unauthenticated `raw.githubusercontent.com` requests, which is what lets a scheduled task (running in a fresh session with no GitHub access configured) read a voice file or keyword list without any connector setup. Nothing sensitive lives here: no credentials, no client data, just style guides, keyword research, and a shared checklist.

## Structure

```
shared/
  on-page-seo.md          15-category, 80+ item on-page SEO checklist. Every skill reads this before generating any page.

bis/
  references/
    voice.md               Tone, audience, decision psychology, banned words
    opinions.md             Hot takes grounded in BIS's actual positioning
    stats.md                Real numbers only — thin by design until Shany supplies more
    stories.md               Real client stories (empty until supplied) + illustrative-scenario rules for blog use
  keywords.csv               BIS blog + service-page keyword research (populated once Ahrefs/manual research runs)
  used-keywords.md           Tracker — primaries already used, don't reuse

vshopper/
  references/
    voice.md, humour.md, stats.md, opinions.md, stories.md   Same shape as bis/, tuned for vShopper's witty B2C voice
  keywords.csv
  used-keywords.md
```

## Who reads this

- **vShopper blog skill** — reads `shared/on-page-seo.md` + everything under `vshopper/`
- **BIS blog skill** — reads `shared/on-page-seo.md` + everything under `bis/`
- **BIS service-page skill** — reads `shared/on-page-seo.md` + everything under `bis/` (service pages lean harder on the Conversion Elements section)

## Editing these files

Voice/opinions/stories files should only change when Shany's actual voice, positioning, or real facts change — not every time a skill runs. `stats.md` and `used-keywords.md` are the ones expected to grow over time as real numbers and used keywords accumulate.
