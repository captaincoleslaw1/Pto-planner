# Time Wiz

The general-public version of the Carrier Dashboard leave calendar — same
planner, no postal anything. Formerly called PTO Planner (renamed Nov 21, 2026).

## How it works (v1.5 — Nov 2026 – Dec 2027)
- Color scheme matches Carrier Dashboard: dark blue (#123a6d) header and
  sticky balance bar, green PTO / blue Sick meters and marks, red holidays.
- Two fillable boxes in a sticky bar that follows you down the page:
  **PTO Balance** and **Sick Balance** (hours), each with the hours left in big
  type and a thin meter of what's left (green PTO, blue Sick).
- Tap a date once: it turns **green = PTO**. Tap again: **blue = Sick**. Tap a
  third time: **red = Holiday**. Fourth tap clears. Every PTO/Sick day subtracts
  **8 hours** from that balance, live in the sticky bar (red if you plan past zero).
- One hint line above the calendar: "Tap once for PTO, twice for Sick,
  three times for Holiday." Under it: "Red = holiday."
- **Third tap = Holiday (red, same as a federal holiday):** for religious or
  other holidays a job gives you. It does not subtract from PTO or Sick.
  A fourth tap clears.
- **Federal holidays are always on** — there is no toggle — and you can tap
  through them like any other day (PTO → Sick → Holiday → **blank** → back
  to the federal holiday in red). The blank stop (an `OFF` mark) is how you
  clear a federal holiday your job doesn't give you; fixed in v1.4 after
  Thomas found you couldn't cycle a federal holiday to blank.
- **Theme button cycles through themes (saved on device), no color picking:**
  Classic (Carrier Dashboard blue), Blush (pink), Lavender, Sage, Peach,
  Ocean, Berry, Sky, and Plain (gray). Each click on the Theme button moves
  to the next one. Theme changes the header, sticky balance bar, page
  background, and borders.
- **Federal holidays are red.** Weekends (Sat/Sun) are shaded and can't be
  marked — most people are already off. No payday markers (those vary by
  employer) and no color/rotation picker (that was the postal schedule).
- v1.5 fixes: the balance card no longer overflows on the right on narrow
  phones (grid panels can now shrink, the balance input flexes to fit), and
  the "Use Holiday for..." explanation paragraph under the hints is removed.
- Balances and marked days are saved on the device (localStorage, key
  `ptoPlanner` kept from v1.0 so existing users keep their data).
- Date boxes are the fat-finger size from the carrier version (14.5px, 32px tall).
- Version number is shown in the header — a lesson from the carrier app.

## Relationship to Carrier Dashboard
Forked from Carrier Dashboard v1.8 (github.com/captaincoleslaw1/Carrier-dashboard)
on Nov 21, 2026, at Thomas's request: "same exact thing but for the general
public — PTO instead of AL." Changes are the renames (AL→PTO, SL→Sick),
weekends-instead-of-Sundays off, federal instead of postal wording, and
dropping the USPS-specific pieces (color rotation, paydays).
