# Game Clock 

Game Clock is just a digital clock, but one that can be manually operated. The main idea is that during some TTRPG game, I may want to have some real-time clock that I can:
* set what looks like a time of day (or just from 0)
* manually change as needed
* have count time in either direction
* allow slower or faster counting

Used Claude to generate initial setup and design. But I wanted to code some features myself. Honestly, this is as much a project I wanted for a specific purpose as it is practicing AI-coding-assistance and UI-tweaking.

## Kanban
This section approximates a kanban board, so I can plan out what I'm doing. 

### TODO
- Fix the bug where you can put it in hours greater than 23 (e.g., set hour to "15" and increase by 10--now you're at 25 o'clock; should instead wrap-around)
- Other buttons can be unified to be much smaller. 
- Add an option to change by how much the clock changes per-second
  - Maybe include double-time, count down, and by-value
  - If we want to do "half"-speed, we need to alter the "how often we add" logic
- Add an option to directly edit the numbers
- Add a reset-to-0 button
- Add time-based alerts?
- 

### In Progress
-

### Done
- Move buttons to above the relevant digits (remove text)
- 
