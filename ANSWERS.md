# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

A process is an independent program that has its own memory space and resources. A thread is a smaller unit of execution that exists inside a process and shares the same memory with other threads. Processes are heavier and take more time to create and manage, while threads are lighter and faster. In this assignment, we used threads because we needed to simulate multiple processes efficiently within one program. Using threads makes it easier to manage scheduling and reduces overhead compared to creating separate processes.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

In Round-Robin scheduling, if a process does not finish within its time quantum, it leaves the CPU and is placed back into the ready queue. This allows other processes to take their turn, ensuring fairness. The process will run again when its turn comes back in the queue. This cycle continues until the process completes its execution.


Example from my output:
```
[Process P1 is running…
Time quantum expired for P1
Process P1 added back to ready queue]
```

**Explanation of example:**
In this example, process P1 started running but did not finish within its time slice. Once the time quantum expired, it was removed from the CPU and returned to the ready queue. This allows other processes to run before P1 gets another chance. This behavior ensures that no single process uses the CPU for too long.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

1. **New**: [P1 is in the New state when the thread is first created using new Thread(P1) but has not started yet.]

2. **Runnable**: [P1 becomes Runnable when the start() method is called and it is ready to be executed by the CPU.
]

3. **Running**: [P1 is in the Running state when the scheduler selects it and it begins executing its run() method.
]

4. **Waiting**: [P1 enters the Waiting state when methods like sleep() are used to simulate execution time, or when it is waiting for its next turn in the ready queue.]

5. **Terminated**: [P1 reaches the Terminated state when it finishes all its execution and no longer needs CPU time.]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [ Web Server ]

**Description**: 
[A web server handles multiple user requests at the same time. Each request can be processed using a separate thread.

**Why Round-Robin works well here**: 
[Round-Robin ensures that each request gets a fair amount of CPU time. This prevents one request from blocking others and keeps the server responsive for all users.]


### Example 2: [Operating System Task Scheduling]

**Description**: 
[Operating systems manage multiple processes like applications, background tasks, and system services.]

**Why Round-Robin works well here**: 
[Round-Robin scheduling ensures that all processes get a fair share of CPU time. It improves responsiveness and prevents any process from dominating the system.]

---

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes
2. How Round-Robin scheduling works
3. Thread lifecycle and states 

**Concepts I need to study more:**
1. Thread synchronization
2. Advanced scheduling algorithms 
