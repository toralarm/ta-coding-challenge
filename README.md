# Coding challenge

Build a small version of TorAlarm: A match list and a match details page.

For inspiration you can download TorAlarm app from here:

  
[https://apps.apple.com/de/app/toralarm-fu%C3%9Fball-ergebnisse/id484990052](https://apps.apple.com/de/app/toralarm-fu%C3%9Fball-ergebnisse/id484990052)  
[https://play.google.com/store/apps/details?id=com.eisterhues_media_2&hl=en](https://play.google.com/store/apps/details?id=com.eisterhues_media_2&hl=en)



The app is deliberately small. The important part of this task, and of the interview, is bug mode: five real incidents from your career, visible in the app, which you will present.

AI assistance is explicitly allowed.
Plan on about 1-2 hours for the implementation and another 2 hours for the incident notes as part of your interview preparation.

## Tech

- Use React for the UI 
- A small Go web server for the backend



### Match list

- Show one day of matches at a time.
- Each match shows the home and away team names
- Previous and next move by one day, limited to today −7 days through today +7 days
- Clicking a match opens its details page



### Match details

- Show the teams, their logos, the score, match status and kickoff
- Should show all goals, cards and subs



### General

- The app is simple, so make sure also deliver a good UX - copying concepts from TorAlarm or other apps is absolutely allowed
- Take care of classical edge cases like no/bad network, failing APIs or invalid data
- You are free to choose any football data API
- Make sure that you provide clear instructions on how to launch your app
- You are free to choose any type of communication between browser and web server



## Design Choices

In the interview you will be asked to explain your decisions on architecture, technology, APIs, data flows and coding style. Please prepare yourself for these kind of questions.

## Bug mode

When the implementation is done, add support for the query parameter `bug-mode=true`. 

With that parameter, the app should contain five or more bugs. 
Each bug is an incident you have seen or caused in your career. If you think that is not doable with the current example app feel free to extend it to accommodate for your bug use case/s.

If you have fewer than five production incidents, say so. You may fill the remaining slots with a public incident write-up you have studied. Mark those clearly as studied.

In the interview you will present each bug. For each one, be ready to answer:

- How is it caused/reproduced?
- How was it caught?
- How long did it exist, and why that long or that short?
- What was the fix?
- How would you rate this fix?
- What was wrong in the engineering flow that led to the bug?

Note: These questions go beyond your code alone. 
We will also cover classical everday engineering challenges (behavorial, cultural ...)