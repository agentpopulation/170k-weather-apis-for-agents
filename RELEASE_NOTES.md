## Weather API endpoints, snapshot 15 Nov 2026

- 177,892 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 8,571 services · 251 country codes · 118,212 keyless JSON rows

### Download

- `Weather_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 177,892 rows, 6.7 MB gzipped (54.6 MB as CSV), SHA-256 `4450a7ec5393f319d4fe893d6e9469fd8a8a424b9225ae6f61befe12400adf29`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Weather_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Weather_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 17,500 · Wrap one URL pattern as a get_forecast tool: pass a place or airport code, return the next hours; add a timeout and a fallback.
- 📱 App features: 65,386 · Show current conditions, air quality and airport weather on a card or a station map.
- 🧠 Grounding and data pipelines: 65,260 · Load climate and observation series on a schedule into your own store for RAG, dashboards and notebooks.
- 🧪 Evals and testing: 177,892 · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

### Changes

- New snapshot: 190,644 endpoints from 9,237 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026; 35,068 more endpoints than the 14 Nov 2026 release (155,576 endpoints from 7,096 services).
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 177,892 endpoints from 8,571 services, 12,752 fewer endpoints than first published under this snapshot (190,644 from 9,237 services), tested 10–15 Nov 2026 (IST).
- Left out: 9 rows whose URL carried a credential-looking parameter or a login.
- Left out: 2 rows with an email-like address.
- Left out: 1,982 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 4 class-exercise copies of the same few ArcGIS Online layers (Miami Beach sea level rise, high-risk areas without shelter, flooded areas, sea level rise and storm surge maps) across many organisations, many with a person's name in the title.
- Left out: 83 layers marked editable in the title (they can hold entries that people added).
- Left out: 280 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 4 rows that passed a data call only from a network location in India.
- Left out: 8,455 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 896 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 26 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 91 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Left out: 229 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 2,553 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 873 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 5,626 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 189 rows that repeat an address already in the pack.
- Overlap: 8,804 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 17,300 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 894 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 1,857 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 5,014 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 1,283 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 5,650 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 468 of these URLs are also in 22k-maritime-apis-for-agents.
- Overlap: 12,567 of these URLs are also in 160k-environment-apis-for-agents.
- Overlap: 19,829 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 1,956 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 117,939 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 2,988 of these URLs are also in 84k-health-apis-for-agents.
- Overlap: 3,348 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 1,432 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 129 of these URLs are also in 4.9k-wildfire-apis-for-agents.
- Overlap: 2,652 of these URLs are also in 67k-energy-apis-for-agents.
- Overlap: 9,952 of these URLs are also in 23k-aviation-apis-for-agents.
- Overlap: 276 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 98 of these URLs are also in 10k-parking-apis-for-agents.
- Overlap: 117 of these URLs are also in 7.8k-earthquake-apis-for-agents.
- Overlap: 45 of these URLs are also in 4.2k-volcano-tsunami-apis-for-agents.
- Overlap: 2 of these URLs are also in 17k-bike-share-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Weather API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
