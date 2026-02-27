# Market Surveillance — Search Query Generator

A lightweight, browser-based tool to automate Google search query generation for market surveillance investigations.

---

## Context & Problem

In market surveillance, investigating suspicious trading activity requires verifying connections between clients involved in transactions — buy side, sell side, and the company or security being traded.

The standard process can involve manually searching Google for each combination of names using exact-match queries (e.g. `"John Smith" "Jane Doe"`), then documenting results. On a case with 10 transactions, this can mean 20–30 individual searches done one by one.

This tool eliminates the manual query-building step entirely.

---

## What It Does

- Input a case ID, a company/security name, and as many buy/sell transactions as needed
- Automatically generates all relevant search combinations :
  - Each buy/sell pair per transaction
  - Each client name against the company/security
- Deduplicates queries — if the same client appears in multiple transactions, redundant searches are removed
- Exports a CSV file with one row per search, including a direct clickable Google URL for each query

---

## How to Use

1. Download `market_surveillance.html`
2. Open it in any web browser (Chrome, Firefox, Edge) — no installation required
3. Fill in the Case ID and Company / Security name
4. Add transactions (buy side name + sell side name)
5. Click **Aperçu** to preview all generated searches
6. Click **Exporter CSV** to download the results file

The exported CSV contains the following columns :

| Column | Description |
|---|---|
| `case_id` | Identifier of the investigation |
| `company` | Company or security name |
| `term_a` | First search term |
| `term_b` | Second search term |
| `search_type` | `buy/sell pair` or `client vs company` |
| `google_query` | The exact query with quotes |
| `google_search_url` | Clickable direct link to Google search |
| `generated_at` | Timestamp of export |

---

## Technical Notes

- Pure HTML/CSS/JavaScript — runs entirely in the browser, no server, no dependencies
- No data is sent anywhere — everything stays local on your machine
- The only external call is loading IBM Plex fonts from Google Fonts on startup
- Compatible with all modern browsers

---

## See Also

→ [`AI_USAGE.md`](./AI_USAGE.md) — transparency note on how AI was used in this project
