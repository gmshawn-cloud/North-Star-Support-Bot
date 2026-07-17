# Scout — North Star Outfitters Support Chatbot

A customer support chatbot built for a fictional outdoor apparel & camping gear
retailer, North Star Outfitters. Handles order tracking, returns & exchanges,
product recommendations, and human handoff, with intent recognition tolerant
of natural phrasing variation.

## How to test

**Live version (no download needed):** open `[LIVE URL GOES HERE]` in any
browser.

**Or run it locally:** download `scout-chatbot.html` and open it directly in
any browser (double-click, or drag it into a browser window). It's a single
self-contained file — no build step, no server, no API keys, no account
creation. Everything runs client-side in plain HTML/CSS/JavaScript.

The chat widget opens automatically over a small mock storefront so it reads
as something actually embedded on a store's site. Use the restart icon
(circular arrow, top-right of the widget) to reset the conversation at any
point.

## Use cases covered

**Order tracking** — Ask to track an order, or just provide an order number.
The bot asks for the number if it wasn't given, then looks it up against the
mock data below.

| Order # | Result |
|---|---|
| 111 | Shipped, arriving tomorrow |
| 222 | Processing, ships within 24 hours |
| 333 | Delivered (bot follows up to check everything arrived okay) |
| anything else | Not found — offered a retry or a handoff to a person |

**Returns & exchanges** — Explains the return policy (30 days from delivery,
unused, original packaging) and provides a returns link. Also recognizes
damage/defect language ("it arrived broken") and routes there directly.

**Product recommendations** — Asks up to two clarifying questions (activity,
then trip length) before recommending a gear category — a 3×4 matrix of
combinations rather than a single canned answer. If the initial message
already states the activity and/or trip length (e.g. "camping trip for 3
days"), it skips straight past whichever question was already answered.

**Human handoff** — Triggered by an explicit request ("talk to a person,"
"connect me with an agent") or automatically offered after a couple of
unrecognized messages in a row. Clearly announces the handoff, simulates a
live agent, and lets the user return to the main bot afterward.

**Fallback handling** — Unrecognized input gets an explicit "didn't catch
that" response with the main options re-shown, escalating to a suggested
handoff if it keeps happening.

## Notes on the implementation

- Vanilla HTML/CSS/JavaScript — no framework or dependencies to install.
- Fonts load from Google Fonts for polish, with system-font fallbacks if
  offline, so functionality never depends on network access.
- All policy text, shipping timelines, and order data match the brief exactly.
- The diamond "blaze trail" under the header tracks progress across the four
  flows (Order / Returns / Gear / Agent) as a visual session indicator.
