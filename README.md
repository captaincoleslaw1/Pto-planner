# PTO Planner

The general-public version of the Carrier Dashboard leave calendar — same
planner, no postal anything.

## How it works (v1.0 — Nov 2026 – Dec 2027)
- Two fillable boxes in a sticky bar that follows you down the page:
  **PTO Balance** and **Sick Balance** (hours), each with the hours left in big
  type and a thin meter of what's left (green PTO, blue Sick).
- Tap a date once: it turns **green = PTO**. Tap again: **blue = Sick**. Tap a
  third time: cleared. Every marked day subtracts **8 hours** from that balance,
  live in the sticky bar (red if you plan past zero).
- One hint line above the calendar: "Tap once for PTO, twice for Sick."
- **Federal holidays are red.** Weekends (Sat/Sun) are shaded and can't be
  marked — most people are already off. No payday markers (those vary by
  employer) and no color/rotation picker (that was the postal schedule).
- Balances and marked days are saved on the device (localStorage).
- Date boxes are the fat-finger size from the carrier version (14.5px, 32px tall).
- Version number is shown in the header — a lesson from the carrier app.

## Relationship to Carrier Dashboard
Forked from Carrier Dashboard v1.8 (github.com/captaincoleslaw1/Carrier-dashboard)
on Nov 21, 2026, at Thomas's request: "same exact thing but for the general
public — PTO instead of AL." Changes are the renames (AL→PTO, SL→Sick),
weekends-instead-of-Sundays off, federal instead of postal wording, and
dropping the USPS-specific pieces (color rotation, paydays).
