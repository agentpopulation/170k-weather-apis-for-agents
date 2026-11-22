# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- New snapshot: 190,644 endpoints from 9,237 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026; 35,068 more endpoints than the 14 Nov 2026 release (155,576 endpoints from 7,096 services).
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 177,892 endpoints from 8,571 services, 12,752 fewer endpoints than first published under this snapshot (190,644 from 9,237 services), tested 10–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Weather_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 170k-weather-apis-for-agents (was 190k-weather-apis-for-agents; first published as weather-api-endpoints). The name follows the count, rounded down.
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

## 2026-11-14 (snapshot-2026-11-14)

- First release: 155,576 endpoints from 7,096 services, tested 10–14 Nov 2026 (IST), snapshot 14 Nov 2026.
- The repository holds a 1,000-row sample and the services list; the full list is the release download Weather_API_Endpoints_AgentPopulation_Snapshot_2026-11-14.csv.gz.
- Left out: 1 listing page that is not a data call.
- Left out: 5 rows whose URL carried a credential-looking parameter or a login.
- Left out: 1,373 ArcGIS Survey123 layers (they can hold people's form answers).
