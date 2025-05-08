# Game Clock 

Game Clock is just a digital clock, but one that can be manually operated. The main idea is that during some TTRPG game, I may want to have some real-time clock that I can:
* set what looks like a time of day (or just from 0)
* manually change as needed
* have count time in either direction
* allow slower or faster counting
* added a `+6 seconds` button (one DnD round)

I used Claude to generate the initial setup and design. But I wanted to code some features myself. Honestly, this is as much a project I wanted for a specific purpose as it is practicing AI-coding-assistance and UI-tweaking.

One edge case that needed some thought was what to do if the hour-ones box was >3 and you moved the hour-tens digit to 2. Should it reset to 00 (what I chose)? An argument could be made that it could prevent the hour-tens digit from changing in that situation. Or to just put you at the equivalent -24 hour (like, 27 would become 03, etc.) 


## Kanban
This section approximates a kanban board, so I can plan out what I'm doing. 

### TODO
- Add some tests
- Add time-based alerts?
- Break these out into separate files? (Meh)


### In Progress
-

### Done
- Restyle the "Interval" input box?
- Refactor digit-fixing code into the commitDigits function?
- Move buttons to above the relevant digits (remove text)
- Fix the bug where you can put it in hours greater than 23 (e.g., set hour to "15" and increase by 10--now you're at 25 o'clock; should instead wrap-around)
- Add an option to directly edit the numbers
- Other buttons can be unified to be much smaller. 
- Add a reset-to-0 button
- - Add an option to change by how much the clock changes per-second
  - if fractional, we show upto 2 decimal places--it's fine for this use case
