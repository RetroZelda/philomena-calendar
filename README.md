# philomena-calendar
Source for [philomena-calendar.org](https://philomena-calendar.org)

This repo is the result of the goal to see how AI can create and calculate a new Calendar and Timezone Offset where everything is relative to an unrelated Belgian techno anthem, Pump Up the Jam.

See: https://youtu.be/-Su287HvJRQ for further details on Philomena Cunk and the PUJT gag.

---

## The Philomena Calendar

A 13-month calendar anchored to **August 18, 1989** — the release date of Technotronic's "Pump Up the Jam" — following the rules of the [International Fixed Calendar](https://en.wikipedia.org/wiki/International_Fixed_Calendar).

- **Year 0, Month 0, Day 0** corresponds to August 18, 1989
- Each year has **13 months of exactly 28 days** (364 days total)
- A **Leap Year Day** is appended at the end of leap years; it belongs to no month
- Years before August 18, 1989 are denoted **BC** ("Before Cunk"), counting backwards
- The 7th month is **Dia** (formerly Sol), renamed in honor of Diane Morgan

### Months

| # | Name |
|---|------|
| 00 | January |
| 01 | February |
| 02 | March |
| 03 | April |
| 04 | May |
| 05 | June |
| 06 | **Dia** *(in honor of Diane Morgan)* |
| 07 | July |
| 08 | August |
| 09 | September |
| 10 | October |
| 11 | November |
| 12 | December |
| ★ | Leap Year Day *(leap years only, belongs to no month)* |

---

## PUJT — Pump Up the Jam Time

A timezone system where **Belgium (GMT+1) is PUJT+0**, making it the center of the world.

- GMT → PUJT-1
- EST → PUJT-6
- CST → PUJT-7
- etc.

---

## The Website

`index.html` is a single-page app that shows:

- **Live PUJT clock** — HH:MM:SS.mmm, ticking in real time, anchored to Belgium GMT+1
- **Today card** — your current Philomena Year (AC/BC), month, day, and a compact date stamp (e.g. `Y36.06.14`)
- **Full 13-month calendar** — scrollable month strip, prev/next month and year navigation, Today button
- **Leap Year Day** — shown as a special amber card on years where the Aug→Aug span contains Feb 29
- **PUJT timezone picker** — common zones pre-listed, auto-selects your local offset

Each calendar cell shows the Philomena day index (0–27) and the corresponding Gregorian date underneath.

---

## Origin

It all started with this prompt to Grok 2:

```
Friday 18 August 1989 was the release date of Belgian act Technotronic's single "Pump Up the Jam".
Can you create a new date/time system based on this gregorian date being sunday, day 0, month 0, and year 0
in a new 13 month year following the rules specified here: https://en.wikipedia.org/wiki/International_Fixed_Calendar
Instead of a gregorian Calendar, we will call this the Philomena Calendar.
And then, can you update all timezones to make Belgian the center point? So since Belgium is GMT+1, can we make
a new timezone system called PUJT(Pump Up the Jam Time) where Belgian is PUJT+1, making GMT be PUJT-1;
EST will become PUJT-6; etc
Finally, can you create an HTML and Javascript webpage that will convert the system's date and time
(including timezone) to display the new Philomena Calendar Date and PUJT TimeZone offset and time
```

---

**13 Month Year sourced from:** [Wikipedia — International Fixed Calendar](https://en.wikipedia.org/wiki/International_Fixed_Calendar)  
**Site Source:** [GitHub — Philomena Calendar](https://github.com/RetroZelda/philomena-calendar)
