# CLAUDE.md — Apitap Team Performance Dashboard
> **READ THIS FIRST** every new session before touching any file.
> Update the `## CURRENT STATE` and `## CHANGELOG` sections with every commit.

---

## PROJECT
Single-file HTML performance dashboard for the Apitap engineering team.
Tracks MantisBT tickets: load, avg resolution time, and reassignment rate per person/month.
Audience: company owner. Language toggle: EN / ES.

- **Live URL:** https://apitap-team-performance.vercel.app
- **Repo:** https://github.com/jimmyriveros/apitap-team-performance.git
- **Deploy:** auto on `git push master` via Vercel–GitHub integration

---

## FILES
```
apitap-team-performance.html   ← entire app (~3300 lines): HTML + CSS + JS in one file
vercel.json                    ← routes / to the HTML file
CLAUDE.md                      ← THIS FILE — context for Claude Code sessions
```

---

## CURRENT STATE
_Last updated: 2026-06-01_

### Period
`1 Nov 2025 — 31 May 2026` | **7 months** | Generated: May 31, 2026

### Global KPIs
| Metric | Value | HTML location |
|--------|-------|---------------|
| Total tickets | **383** | `data-count="383"` on first `.value` in `.kpi-band` |
| Completed | **379** | `data-count="379"` on second `.value` |
| Still open | **4** | `data-count="4"` on third `.value` |
| Resolved (tooltip) | 271 | `.td-val` in completed tip-box |
| Closed (tooltip) | 108 | `.td-val` in completed tip-box |
| % completed (tooltip) | 99% | `.td-val` in completed tip-box |

### PEOPLE — Current Values
| Name | total | periods | avg | ratio |
|------|-------|---------|-----|-------|
| Diego | 170 | 181 | 3d, 3h | 1.06 |
| Jesús | 109 | 129 | 10d, 23h | 1.18 |
| Otoniel | 101 | 127 | 3d, 18h | 1.26 |
| Ashish | 71 | 72 | 10d, 15h | 1.01 |
| SumitK | 52 | 55 | 5d, 2h | 1.06 |
| Semyon | 21 | 25 | 9d, 3h | 1.19 |
| Luis | 12 | 12 | 2d | 1.00 |

### PEOPLE — Monthly Breakdown (full months[] arrays)
Months order: Nov/2025, Dic/2025, Ene/2026, Feb/2026, Mar/2026, Abr/2026, May/2026

**Diego** (total:170, periods:181, avg:'3d, 3h', ratio:1.06)
| Month | tickets | periods | avg | ratio |
|-------|---------|---------|-----|-------|
| Nov 2025 | 25 | 25 | 3d, 19h | 1.00 |
| Dic 2025 | 23 | 23 | 1d, 22h | 1.00 |
| Ene 2026 | 20 | 20 | 5d, 9h | 1.00 |
| Feb 2026 | 32 | 32 | 4d, 2h | 1.00 |
| Mar 2026 | 32 | 32 | 2d, 2h | 1.00 |
| Abr 2026 | 18 | 19 | 1d, 23h | 1.06 |
| May 2026 | 23 | 31 | 2d, 16h | 1.35 |

**Jesús** (total:109, periods:129, avg:'10d, 23h', ratio:1.18)
| Month | tickets | periods | avg | ratio |
|-------|---------|---------|-----|-------|
| Nov 2025 | 1 | 1 | 5h | 1.00 |
| Dic 2025 | 0 | 0 | — | 0 |
| Ene 2026 | 2 | 2 | 2m, 9d, 12h | 1.00 |
| Feb 2026 | 38 | 38 | 21d, 20h | 1.00 |
| Mar 2026 | 30 | 31 | 8d, 17h | 1.03 |
| Abr 2026 | 37 | 44 | 3d, 15h | 1.19 |
| May 2026 | 12 | 14 | 1d, 5h | 1.17 |

**Otoniel** (total:101, periods:127, avg:'3d, 18h', ratio:1.26) — NOT in May report, values unchanged
| Month | tickets | periods | avg | ratio |
|-------|---------|---------|-----|-------|
| Nov 2025 | 0 | 0 | — | 0 |
| Dic 2025 | 0 | 0 | — | 0 |
| Ene 2026 | 0 | 0 | — | 0 |
| Feb 2026 | 1 | 1 | — | 1.00 |
| Mar 2026 | 54 | 59 | 5d, 23h | 1.04 |
| Abr 2026 | 49 | 62 | 2d, 13h | 1.24 |
| May 2026 | 7 | 7 | 1d, 2h | 1.00 |

**Ashish** (total:71, periods:72, avg:'10d, 15h', ratio:1.01)
| Month | tickets | periods | avg | ratio |
|-------|---------|---------|-----|-------|
| Nov 2025 | 10 | 10 | 16d, 7h | 1.00 |
| Dic 2025 | 8 | 8 | 16d, 5h | 1.00 |
| Ene 2026 | 5 | 5 | 7d, 16h | 1.00 |
| Feb 2026 | 7 | 7 | 22d, 5h | 1.00 |
| Mar 2026 | 16 | 16 | 4d, 5h | 1.00 |
| Abr 2026 | 14 | 14 | 6d, 14h | 1.00 |
| May 2026 | 12 | 12 | 6d, 13h | 1.00 |

**SumitK** (total:52, periods:55, avg:'5d, 2h', ratio:1.06)
| Month | tickets | periods | avg | ratio |
|-------|---------|---------|-----|-------|
| Nov 2025 | 0 | 0 | — | 0 |
| Dic 2025 | 3 | 3 | 1m, 3d, 10h | 1.00 |
| Ene 2026 | 2 | 2 | 3d, 1h | 1.00 |
| Feb 2026 | 3 | 3 | 4d, 22h | 1.00 |
| Mar 2026 | 19 | 20 | 4d, 10h | 1.05 |
| Abr 2026 | 19 | 19 | 2d, 20h | 1.00 |
| May 2026 | 10 | 10 | 2d, 9h | 1.00 |

**Semyon** (total:21, periods:25, avg:'9d, 3h', ratio:1.19) — no May activity
| Month | tickets | periods | avg | ratio |
|-------|---------|---------|-----|-------|
| Nov–Feb | 0 | 0 | — | 0 |
| Mar 2026 | 12 | 13 | 3d | 1.08 |
| Abr 2026 | 10 | 11 | 16d, 11h | 1.10 |
| May 2026 | 0 | 0 | — | 0 |

**Luis** (total:12, periods:12, avg:'2d', ratio:1.00)
| Month | tickets | periods | avg | ratio |
|-------|---------|---------|-----|-------|
| Nov–Feb | 0 | 0 | — | 0 |
| Mar 2026 | 4 | 4 | 3d | 1.00 |
| Abr 2026 | 2 | 2 | 3h | 1.00 |
| May 2026 | 6 | 6 | 1d, 22h | 1.00 |

### Open Tickets at May 31, 2026 (OPEN_TICKETS array)
| ID | Title | Assignee | assigned |
|----|-------|----------|----------|
| 1735 | Crash provoked when clicking on records of Payment Account Summary of a Consumer | Otoniel | 2026-05-14 |
| 1740 | Push notifications should be generated for all message types. | Ashish | 2026-05-12 |
| 1759 | Promotions search does not show promotions | SumitK | 2026-05-27 |
| 1761 | Messages sent by the consumer are not displayed | Ashish | 2026-05-26 |

### Ticket ID Range by Month (reference for new IDs)
| Period | ID range (approx) |
|--------|-------------------|
| Nov 2025 | 1373–1408 |
| Dic 2025 | 1409–1438 |
| Ene 2026 | 1444–1475 |
| Feb 2026 | 1487–1544 |
| Mar 2026 | 1551–1638 |
| Abr 2026 | 1619–1700 |
| May 2026 | 1701–1763 |

---

## DATA ARCHITECTURE

### PEOPLE array — schema
```js
// Location: const PEOPLE = [...] in <script>
{
  name: 'Diego',          // string — MUST match key in TICKET_DATA exactly
  total: 170,             // unique tickets in full period
  periods: 181,           // total assignment periods (total + reasign bouncebacks)
  avg: '3d, 3h',          // overall avg time — format: 'Xm, Xd, Xh' | 'Xd, Xh' | 'Xh' | '<1h' | '—'
  ratio: 1.06,            // periods/total — 2 decimal places
  months: [               // EXACTLY 7 entries, one per month in order
    { m:'Nov', y:'2025', tickets:25, periods:25, avg:'3d, 19h', ratio:1.00 },
    // ...
    { m:'May', y:'2026', tickets:23, periods:31, avg:'2d, 16h', ratio:1.35 }
  ]
}
```
**Month key values:** `m` uses Spanish abbreviations: `Nov`, `Dic`, `Ene`, `Feb`, `Mar`, `Abr`, `May`
**Year values:** `y:'2025'` for Nov+Dic, `y:'2026'` for Ene–May
**Zero month:** `{ m:'Nov', y:'2025', tickets:0, periods:0, avg:'—', ratio:0 }`

### OPEN_TICKETS array — schema
```js
// Location: const OPEN_TICKETS = [...]
{
  name: 'Ashish',    // must match PEOPLE[].name
  count: 2,          // MUST equal tickets.length
  tickets: [
    {
      id: '0001740',                    // 7-digit zero-padded string
      title: 'Push notifications...',   // full ticket title
      assigned: '2026-05-12',           // date assigned (YYYY-MM-DD)
      url: 'https://www.atlallc.com/mantisbt/view.php?id=1740'
    }
  ]
}
// persons with count:0 must still appear in array with tickets:[]
```

### TICKET_DATA object — schema
```js
// Location: const TICKET_DATA = {...}  (~line 1756)
'Diego': {
  'Nov 2025': [ {id:'0001375', title:'...', url:'...'}, ... ],
  'Dic 2025': [...],
  'Ene 2026': [...],
  'Feb 2026': [...],
  'Mar 2026': [...],
  'Abr 2026': [...],
  'May 2026': [...],
}
```
- Month key format: `'MMM YYYY'` using Spanish abbreviations
- `id`: 7-digit zero-padded string `'0001735'`
- `url`: `'https://www.atlallc.com/mantisbt/view.php?id=NNNN'`
- Contains ALL tickets the person worked on (including reasigned from others)
- A ticket ID can appear in multiple people's data (reasignation chains)
- **Never delete** existing entries — only append new ones

---

## UPDATE PROCEDURE (follow in order when new month data arrives)

### 0. Always read this file first
If opening a new session: `Read CLAUDE.md` → you now have full context.

### 1. Identify what's new
```
new_tickets_for_person = report_tickets − tickets_already_in_TICKET_DATA[person]['May YYYY']
```
Check by ticket ID. Keep existing, add new.

### 2. Update TICKET_DATA (append only)
Add new ticket entries to the person's month key. Example:
```js
'May 2026': [
  // ...existing tickets...
  {id:'0001764', title:'New bug title', url:'https://www.atlallc.com/mantisbt/view.php?id=1764'},
]
```

### 3. Update PEOPLE months[] entry for that month
Replace the month object with new authoritative values from report:
```js
{ m:'May', y:'2026', tickets: NEW_T, periods: NEW_P, avg: 'Xd, Xh', ratio: NEW_P/NEW_T }
```

### 4. Recalculate PEOPLE top-level stats
```
delta_tickets = new_may_tickets − old_may_tickets
delta_periods = new_may_periods − old_may_periods

new_total   = old_total + delta_tickets
new_periods = old_periods + delta_periods
new_ratio   = round(new_periods / new_total, 2)

// Weighted avg recalculation:
old_total_hours  = old_total × hours(old_avg)
old_may_hours    = old_may_tickets × hours(old_may_avg)
base_hours       = old_total_hours − old_may_hours
new_total_hours  = base_hours + (new_may_tickets × hours(new_may_avg))
new_avg          = new_total_hours / new_total  → format to 'Xd, Xh'
```
`hours()`: m×720 + d×24 + h

### 5. Update OPEN_TICKETS
Replace entire array with only tickets confirmed open at new cutoff.
- Report will explicitly list open tickets at period end
- People with no open tickets: `{ name, count:0, tickets:[] }`

### 6. Update global KPIs
```
new_global_total   = old_global_total + count(truly_new_ticket_IDs_not_in_any_person_data)
new_open           = count(all open tickets in new OPEN_TICKETS)
new_completed      = new_global_total − new_open

// Tooltip split (approx 71% resolved / 29% closed):
resolved ≈ round(new_completed × 0.71)
closed   = new_completed − resolved
pct      = round(new_completed / new_global_total × 100) + '%'
```

### 7. Update all date/text strings
**HTML direct (not i18n):**
- Hero stamp period: `<div class="v">1 Nov 2025 — DD MMM YYYY</div>`
- KPI `data-count` on three `.value` elements
- Footer: `<p>DD MMM YYYY</p>` and `<p>N meses</p>`
- Tooltip resolved/closed/% values

**i18n strings (update in BOTH `en:{}` and `es:{}`):**
```
nav_badge           → 'Report · May 31, 2026'
hero_lede           → update ticket count + date
stamp_generated_v   → 'May 31, 2026' / '31 de Mayo 2026'
kpi_eyebrow_right   → 'NNN tickets · Nov 2025 — May 2026'
kpi_open_unit       → 'tickets in progress as of May 31'
tip_open_body       → update date + count
ot_eyebrow          → 'Open tickets as of May 31, 2026'
ot_title_pre        → 'N tickets'
ot_lede             → update date
gt1_ex              → 'Diego: <span>NNN tickets</span>...'
gt2_desc            → update date in 'or until...'
footer_coverage_tickets → 'NNN total tickets'
footer_status_resolved  → 'NNN resolved or closed'
footer_status_open      → 'N still open'
ot_detail_eyebrow   → '— Open tickets as of May 31, 2026'
detail_tip_avg_body → 'or until May 31 2026 if still open'
```

### 8. Update CLAUDE.md
- Update `## CURRENT STATE` with new values
- Add entry to `## CHANGELOG`

### 9. Commit and push
```bash
git add apitap-team-performance.html CLAUDE.md
git commit -m "Update report to [DATE] — [brief summary]"
git push origin master
# Vercel auto-deploys on push
```

---

## SECTION MAP (page layout → data source)

| # | Section name | Data source | Key strings to update |
|---|-------------|-------------|----------------------|
| 01 | KPI band (3 counters) | Global KPIs | `data-count`, tooltip values |
| 02 | Open tickets grid | `OPEN_TICKETS[]` | `ot_*` i18n keys, count/date |
| 03 | Metrics Glossary | static + i18n | `gt1_ex` (Diego count), `gt2_desc` (date) |
| 04 | Team list (bars) | `PEOPLE[]` | person row: total, avg, ratio |
| 05 | Individual detail | `PEOPLE[]` + `TICKET_DATA` | month stats + ticket drawer |
| 06 | Compare section | `PEOPLE[]` | auto-reads from PEOPLE array |
| — | Nav badge | i18n `nav_badge` | date string |
| — | Hero subtitle | i18n `hero_lede`, stamps | ticket count + dates |
| — | Footer | i18n `footer_*` + hardcoded | counts, period dates |

---

## CALCULATION REFERENCE

### Hours parser (used in step 4)
```
'3d, 4h'        → 3×24 + 4  = 76h
'1m, 9d, 12h'   → 1×720 + 9×24 + 12 = 948h
'22h'           → 22h
'2d'            → 48h
'—'             → 0 (skip from weighted avg)
```

### Hours formatter (inverse)
```
h < 24         → 'Xh'
24 ≤ h < 720   → 'Xd, Xh'  (if remainder ≥ 1h, else 'Xd')
h ≥ 720        → 'Xm, Xd, Xh'
```

### Ratio formula
```
ratio = total_periods / unique_tickets   (round to 2 decimals)
1.00 = no reasignation bouncebacks
>1.00 = some tickets came back to person
```

### Months count
Nov 2025 = month 1 → May 2026 = month 7 → "seven months" / "siete meses"
When a new month is added beyond May 2026, update `h1_w6`/`h1_w7` and `footer_months`.

---

## IMPORTANT NOTES

1. **TICKET_DATA is for display only.** The drawer shows ticket links. The PEOPLE stats are authoritative — PEOPLE and TICKET_DATA can be slightly inconsistent in counts (tickets reasigned across people appear in multiple TICKET_DATA entries but count once in PEOPLE.total).

2. **Never delete tickets from TICKET_DATA.** Only append. Even if a ticket doesn't appear in the new report, keep it.

3. **Otoniel, Semyon** have no primary tickets from the May report. Their PEOPLE data stays unchanged unless a report explicitly includes them.

4. **Month ordering in PEOPLE.months[]** must always be exactly 7 entries in chronological order: Nov/2025, Dic/2025, Ene/2026, Feb/2026, Mar/2026, Abr/2026, May/2026. When June data arrives, add an 8th entry and update h1 text to "eight months."

5. **i18n system:** The page defaults to English on load. The `es:{}` block provides Spanish translations. Both blocks MUST be updated together. Hardcoded HTML defaults (visible before JS runs) should also be updated.

6. **git identity** (this machine): email `jimmyriveros14@gmail.com`, name `jimmyriveros` (set per-repo, already configured).

---

## CHANGELOG

| Date | Period | Tickets | Description |
|------|--------|---------|-------------|
| 2026-05-08 | Nov 2025–May 8, 2026 | 344 total / 334 done / 10 open | Initial report |
| 2026-06-01 | Nov 2025–May 31, 2026 | 383 total / 379 done / 4 open | Full May update: +19 Diego, +9 Jesús, +6 Ashish, +4 Luis, +1 SumitK. Open: #1735 Otoniel, #1740/#1761 Ashish, #1759 SumitK |
