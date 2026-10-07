# Coding challenge

Build a small version of TorAlarm: a match list and a match details page.

The app is deliberately small. The important part of this task, and of the interview, is bug mode: five real incidents from your career, visible in the app, which you will present.

AI assistance is explicitely allowed.

Plan on about 4–6 hours for the build. The incident notes are interview preparation, separate from that time.

## What to build

Use React for the UI and a small Go web server for the backend.

The browser talks only to your Go server. The server exposes two endpoints: matches for one date, and a single match by id. It owns the data source, the date window, and any caching. The browser never calls a football API directly and never sees an API key.

Use any API that can deliver football results, or commit fixture files and serve those. A reviewer must be able to start the app with one command and no secrets. Document the Go and Node versions and that command. Do not commit API keys.

### Match list

- Show one day of matches at a time.
- Each match shows the home and away team names and crests. Use a fallback when a crest is missing.
- Previous and next move by one day, limited to today −7 days through today +7 days.
- Clicking a match opens its details page.

### Match details

- Score for both sides, and the match status: scheduled, live, finished, or postponed.
- Events. Each event has a minute, a type, a team, and a short label. Always show goals. Show cards and substitutions when the data includes them.
- Kick-off time. Store it in UTC and display it in the viewer's local timezone, and show that the original time was UTC.

### While using it

- Also take care of classical edge cases like no/bad network, failing APIs or invalid data

## Bug mode

When the implementation above is done, support the query parameter `bug-mode=true`. 

With that parameter, the app should contain five or more bugs. 
Each bug is an incident you have seen or caused in your career. If you feel that is not doable with the current example app feel free to extend it to accomodate for your bug use case.

If you have fewer than five production incidents, say so. You may fill the remaining slots with a public incident write-up you have studied. Mark those clearly as studied.

In the interview you will present each bug. For each one, be ready to answer:

- How is caused/reproduced?
- How was it caught?
- How long did it exist, and why that long or that short?
- What was the fix?
- How would you rate this fix?
- What was wrong in the engineering flow that led to the bug?
