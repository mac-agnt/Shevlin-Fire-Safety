# Pulse demo script: Shevlin Fire Safety

## Start and stop

1. Double-click **Start Demo.command**. Chrome opens at **http://pulse.localhost:8080**.
2. Close that Terminal window when you're done. That stops the demo.

The first time, macOS may ask whether Terminal can access your Downloads folder: click **Allow**.
No internet needed; React and the fonts are bundled in `vendor/`.

## The story on every screen

Three threads, with the same numbers on Home, the Briefing agent, Work and Activity:

- **Paperwork:** 3 finished jobs, 412 extinguishers, €3,850 not invoiced. Each pack (asset list, service report, IS 291 certificate, invoice) is built in 30 seconds once a job is marked complete.
- **Renewals:** 14 annual services due in the next 30 days. 6 not booked, worth €4,200. 2 already overdue.
- **Diary:** 3 schedule changes this week never reached a technician's diary. Today's missed one: Dublin city centre, 2pm.

The business: 4 staff, 86 service contracts, 4,120 extinguishers under management, €7,300 owed in.

## The five screens

| Pain | Where | What to show |
|---|---|---|
| Gary types every extinguisher into WhatsApp | Service › Site Walk | Pick Pass, add a photo, log the last extinguisher, then **Complete job** |
| An hour per 190 extinguishers of paperwork | Service › Certificates | The pack from the walk lands here, built in 30 seconds |
| Service dates in a paper notebook | Service › Renewals | 14 due, 6 amber, 2 red, the reminder ready to send |
| A rescheduled job never reached Gary's diary | Work › Schedules | The 3 diary changes, and **Push** on each |
| 3,000 extinguishers at one site | Service › Asset Register | Ashtown Hospital Campus: scroll all 3,000 rows |

Also new: **Records › Sites** (the 86 sites on a map; click a pin) and **Dashboard › Pipeline**.

## Questions Helios answers

Type these on Home, or click the matching suggestion. The wording can change; Helios listens for the key words.

| Ask | Helios shows | Key words it listens for |
|---|---|---|
| What's waiting on paperwork? | 3 jobs, 412 extinguishers, €3,850, and the three packs | paperwork, certificates, packs, invoiced |
| Which renewals aren't booked? | 14 due, 6 not booked worth €4,200, 2 overdue | renewals, booked |
| What changed in the diary this week? | The 3 changes, today's 2pm at Parliament Chambers | diary, rescheduled, moved, 2pm |
| Who owes us money? | €7,300 across 4 customers, Grafton Arcade first | owe, owed, money, overdue |
| How many extinguishers at the hospital? | Ashtown Hospital Campus, block by block | hospital, Ashtown, extinguishers, register |

Follow-ups offered as buttons: **Send all 3 packs**, **Draft the renewal reminders**, **Push them to the diaries**, **Draft chase emails**. Each stops at a **NEEDS YOUR YES** card. **Confirm** carries it out, and the pages update: send the packs and Home's inbox and Certificates both drop them.

Anything else gets: "Everything I reach goes through a registered tool with a declared permission, and none of them covers that question yet." It then offers buttons for the questions above.

## Watch out for

- **Complete job** only arms once all 26 extinguishers are logged. The demo opens at 25 of 26: pick Pass, then **Log extinguisher 26**.
- Completing the walk adds a fourth pack (438 extinguishers, €4,214). Reload the page to get back to 3, 412 and €3,850.
- The briefing is the 07:00 message, so it keeps the morning's numbers after you complete or send anything.
- **Old link:** `localhost:8080/Pulse%20v4%20Glass.dc.html` no longer works. Use http://pulse.localhost:8080.
