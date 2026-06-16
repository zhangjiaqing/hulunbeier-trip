# AGENT.md

This project is a static shareable family travel plan for a Hulunbeier self-drive trip.

The user is planning a summer 2026 family trip from Nanjing to Hailar, with 4 adults and 2 children as the baseline local-travel group. Flight budgeting only covers 3 adults and 2 children. The target total budget is under RMB 20,000. The flights are now booked for July 14-20, 2026, making this a fixed 7-day / 6-night itinerary.

## Project Files

- `index.html`: canonical GitHub Pages entry file. Keep this as the primary published page.
- `呼伦贝尔家庭自驾旅行分享版.html`: local/share copy of the same page. Keep it byte-for-byte identical to `index.html` unless the user explicitly wants two versions.
- `呼伦贝尔家庭自驾旅行初版方案.md`: text planning source and notes. Keep major route, lodging, equipment, and budget decisions aligned with the HTML.
- `assets/`: image assets used by the HTML page.
  - `route-map.png`: current route map image.
  - `hero-grassland.png`, `wetland-sunset.png`, `manzhouli-night.png`, `reindeer-family.png`: visual assets for the page.

## Current Route Decision

Booked flights:

- Outbound: 2026-07-14, XiamenAir MF8587, Nanjing Lukou T1 departure 12:45, expected Hailar Dongshan arrival around 16:00.
- Return: 2026-07-20, Juneyao Air HO2242, Hailar Dongshan T2 departure 13:15, expected Nanjing arrival around 16:35.
- Local Calendar: these two flight events were added to the macOS Calendar app in the `家庭` calendar with 24-hour and 3-hour display reminders.
- Flight monitoring was deleted after ticket purchase. Future work should focus on rental cars and city/town hotels unless the user explicitly asks to monitor flights again.

Current recommended route is a non-crossing north loop:

1. D1: Nanjing -> Hailar. Arrive, pick up car, supplies, sleep in Hailar city.
2. D2: Hailar -> Morigele River -> Erguna Wetland -> Erguna. Sleep in Erguna city.
3. D3: Erguna -> Genhe -> Aoluguya Reindeer Tribe. Reindeer feeding is a must-have child-focused stop. Sleep in Genhe city.
4. D4: Genhe -> Mordaoga forest section -> Enhe/Shiwei. Forest and border-town day. Sleep in Enhe or Shiwei town.
5. D5: Enhe/Shiwei -> Heishantou short horse ride / light herder experience -> 186 Ribbon River -> Manzhouli. Sleep in Manzhouli city.
6. D6: Manzhouli -> Hulun Lake / Zhalainuoer -> Hailar. Sleep in Hailar city.
7. D7: Hailar -> Nanjing. Return logistics only; plan airport car return/check-in around 10:30 for the 13:15 HO2242 flight.

Rationale: this replaced the previous crossing-looking route by swapping D3 and D4. Later, after flights were booked, the final two days were adjusted so the family does not need to leave Manzhouli around 7:00 on the 13:15 return-flight day. Heishantou is now a short stop rather than an overnight base; D5 pushes on to Manzhouli for night views, and D6 returns to Hailar after Hulun Lake/Zhalainuoer.

## Non-Negotiable User Preferences

- Include Aoluguya reindeer feeding.
- Do not arrange lodging inside scenic areas. Use city/town lodging instead.
- Do not book Heishantou lodging in the current plan unless the user explicitly reopens that tradeoff. Heishantou is currently a short horse-riding / herder-experience stop, not an overnight stop.
- Prefer paved roads, official scenic-area roads, and town/city bases.
- MPV is acceptable only for conventional paved-road routing. Avoid grassland tracks, pasture roads, rainy dirt roads, unknown shortcuts, and night driving on grassland sections.
- Do not add Arxan or far detours unless the user explicitly chooses a longer trip.
- Keep the plan child-friendly for a 9-year-old and a 5-year-old.
- Keep commercial/travel-agency video material as reference only. Do not turn the page into a tour advertisement.

## Video References Already Incorporated

The user referenced these Bilibili videos:

- `https://www.bilibili.com/video/BV1Ps7y62E9D/`
- `https://www.bilibili.com/video/BV1xh5T6KEyD/`

What was publicly verifiable:

- The first video title/description/chapters cover Morigele, Erguna, Genhe/Aoluguya, Mordaoga/Shiwei/Linjiang, Enhe, Heishantou, Manzhouli, and Hulun Lake. This supported using a complete north-loop structure.
- The second video title emphasizes not rushing attractions even in a 6-day plan. Public comments included a similar direction: Hailar, Morigele, Wulan Mountain / Erguna River, birch forest, Enhe, G331 / border route, Manzhouli.
- Public subtitles were not available via the readable interfaces at the time. Do not claim transcript-level details unless you re-verify them.

## Flight Status

Flight monitoring is inactive. The recurring heartbeat automation named `南京往返海拉尔直飞机票监控` was deleted on 2026-06-16 after tickets were purchased.

If the user explicitly asks to restart monitoring, use these historical constraints:

- Route: Nanjing Lukou `NKG` to Hailar Dongshan `HLD`, round trip.
- Date window: 2026-07-01 to 2026-08-15.
- Trip length: return interval must be 6 or 7 days.
- Direct flights only. Do not include transfers, stopovers that require changing flights, or multi-segment routes.
- Estimate for 3 adults + 2 children; if child fares are unclear, conservatively use adult fare and state that assumption.
- Notify immediately if estimated average per person is under RMB 2,200.
- Only read and summarize prices. Do not enter passenger details, place orders, or submit bookings.
- Current Chrome/browser safety policy blocks reading `flights.ctrip.com` and `www.fliggy.com`; do not use Ctrip/Trip.com or Fliggy pages or try to bypass that restriction. Use allowed channels such as Qunar, Tongcheng, airline official channels, or ordinary search results.
- Flight prices are highly time-sensitive. Never treat old snapshots in the page as current without rechecking.

Current planning priority:

- Rental car: compare GL8 / Trumpchi M8 / 7-seat SUV inventory for July 15 morning pickup versus July 14 arrival pickup, and July 20 return before airport check-in. If July 14 arrival pickup and July 15 morning pickup both price as the same number of rental days, prefer arrival-day pickup for convenience.
- Hotels: lock refundable city/town lodging for Hailar twice (D1 and D6), Erguna, Genhe, Enhe/Shiwei, and Manzhouli. Do not include a Heishantou overnight in the current baseline.
- Budget: the actual flight total has not been recorded in the project yet. Do not invent it; ask the user or leave it as "按实际订单补录".

## Editing Rules

- Keep `index.html` and `呼伦贝尔家庭自驾旅行分享版.html` synchronized. After editing, run:

```bash
cmp -s index.html 呼伦贝尔家庭自驾旅行分享版.html
```

- When updating the route, update all of these together:
  - route cards
  - route map image and alt text
  - timeline day cards
  - lodging table order
  - equipment/notes if affected
  - Markdown source plan
- For image assets intended for the site, store final files under `assets/`.
- For route maps, do not rely on image generation for Chinese labels. Use generated or searched imagery only as a background if needed, then place route lines and Chinese text locally with deterministic tools.
- Route-map geography should keep:
  - China-Russia border / Erguna River on the west or left side.
  - Hailar on the east side.
  - Manzhouli in the southwest/west.
  - Genhe/Aoluguya in the northeast/forest direction.
  - Enhe/Shiwei near the northwest border-town section.
- Do not use decorative SVG/orb backgrounds or marketing-only sections. This is a practical family itinerary page.

## Verification Checklist

Before finishing a meaningful change:

```bash
git status -sb
cmp -s index.html 呼伦贝尔家庭自驾旅行分享版.html
file assets/route-map.png
rg -n "已出票航班|MF8587|HO2242|视频参考后的调整|必要装备" index.html 呼伦贝尔家庭自驾旅行初版方案.md
```

For visual QA, prefer serving over localhost instead of opening `file://` if Browser automation blocks local-file access:

```bash
python3 -m http.server 8765
```

Then open:

```text
http://127.0.0.1:8765/index.html#route
```

Stop the temporary server when done.

## Publishing

Git remote:

```text
git@github.com:zhangjiaqing/hulunbeier-trip.git
```

Branch:

```text
main
```

Only commit and push when the user asks to publish or when the current task clearly continues the GitHub Pages publishing workflow. Use concise commit messages such as:

```text
Refine Hulunbeier loop route
Update trip planning notes
```

After pushing, verify `git status -sb` shows `main...origin/main` with no local changes.
