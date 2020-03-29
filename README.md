# a-scheduling-program-to-implements-a-Queue-with-two-levels
17. Design a scheduling program to implements a Queue with two levels: 
Level 1: Fixed priority Preemptive Scheduling 
Level 2: Round Robin Scheduling 
For a Fixed priority Preemptive Scheduling (Queue1), the Priority 0 is highest priority. If one process P1 is scheduled and running, another process P2 with higher priority comes. The New process (high  priority) process P2 Preempts currently running process P1 and process P1 will go to second level queue. Time for which process will strictly execute must be considered in the multiples of 2. All the processes in second level queue will complete their execution according to round robin scheduling. Consider: 
1. Queue 2 will be processed after Queue 1 becomes empty.  
2. Priority of Queue 2 has lower priority than in Queue 1.

Description:-
This application implements Multilevel Feedback Queue in C++ with two levels:
Level 1: Fixed priority Preemptive Scheduling
Level 2: Round Robin Scheduling
1. Fixed priority Preemptive Scheduling (Queue 1)
 * Priority 0 is highest priority.
 * Quantum:  4unit time
 * Preemptive:
If one process e.g. P1 is scheduled and running, now another process with higher priority comes e.g. P2. New process (high priority) process P2 Preempts currently running process P1 and process P1 will go to second level queue.
2. Round Robin Scheduling (Queue 2)
* Quantum: 4 unit time
* All the processes in second level queue will complete their execution according to round robin scheduling.
* Queue 2 will be processed after Queue 1 becomes empty.
* Priority of Queue 2 has lower priority than in Queue 1.
Suppose Queue 1 is empty and currently process from Queue 2 is being executed. Now, If at this time a new process arrives then new process will be part of Queue 1. So, new
process should be scheduled as Queue 1 has higher priority than Queue 2. Again after Queue 1 becomes empty Queue 2 will resume execution.


 INPUT FORMAT:<Pid, Arrival_time, Burst_time,Priority>
OUTPUT FORMAT:<Pid Response_Time Finish_Time Waiting_Time >
