# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Your Development Log:

### Entry 1 - [ March 28, 2026 - 11:00 PM]
**What I did**:  I started the assignment, forked the repository, renamed it, updated my student ID (444052900) in the code and Compiled and ran the program successfully

**Challenges**: At first I was confused about how GitHub and Git worked together.

**Solution**: I followed the instructions carefully and tested the repository setup step by step

**Time spent**: about 1 hour

---

### Entry 2 - [March 29, 2026 - 01:00 AM]
**What I did**: I implemented Feature 1 by adding priority to the Process class and displaying it when the process enters the ready queue.

**Challenges**: I was not sure where to place the priority code and how to print it correctly.

**Solution**: I reviewed the Process class and addProcessToQueue method, then tested the output until it worked correctly.

**Time spent**: about 30 minutes 

---

### Entry 3 - [March 29, 2026 - 01:30 AM]
**What I did**: I implemented Feature 2 by adding a static counter for context switches

**Challenges**: I needed to understand exactly when a context switch should be counted

**Solution**: I added the counter in SchedulerSimulation and incremented it whenever a new process started running

**Time spent**: about 30 minutes 

---

### Entry 4 - [March 29, 2026 - 03:30 pM]
**What I did**:  I implemented Feature 3 by tracking waiting time and preparing the summary table.

**Challenges**: Calculating waiting time and printing the summary table correctly was the hardest part

**Solution**: I used System.currentTimeMillis() and stored all processes in a list so I could print the final summary.

**Time spent**: about 1 hour

---

### Entry 5 - [March 29, 2026 - 05:00 pM]
**What I did**: I tested the full program output and fixed formatting and Git issues. 

**Challenges**: I had trouble with terminal symbols, Git commits, and making sure the output looked correct.

**Solution**: I re-ran the program multiple times, corrected the code, and pushed the final version to GitHub.

**Time spent**: about 1.5 hour

---


## Summary

**Total time spent on assignment**: [4 hours]

**Most challenging part**: The most challenging part was calculating the waiting time and printing the summary table correctly. It was difficult to track the process timing and organize the final output in a clear format. I also found Git commits a bit confusing at the beginning.

**Most interesting learning**: The most interesting part was understanding how Round-Robin scheduling works in practice. I liked seeing how processes move in and out of the ready queue and how threads are managed using Java methods like start(), sleep(), and join().

**What I would do differently next time**: Next time, I would start earlier and plan my work more clearly. I would also make commits after each small step to better track my progress. This would help me avoid confusion and make debugging easier.
