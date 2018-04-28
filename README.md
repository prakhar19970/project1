# project1
This project is about scheduling 
The question assigned to me is
Ques. 7. Design a scheduling program to implements a Queue with two levels:
 Level 1 : Fixed priority preemptive Scheduling 
Level 2 : Round Robin Scheduling
 For a Fixed priority preemptive Scheduling (Queue 1), the Priority 0 is highest priority. If one process P1 is scheduled and running , another process P2 with higher priority comes. The New process (high priority) process P2 preempts currently running process P1 and process P1 will go to second level queue. Time for which process will strictly execute must be considered in the multiples of 2.. All the processes in second level queue will complete their execution according to round robin scheduling. Consider: 1. Queue 2 will be processed after Queue 1 becomes empty. 2. Priority of Queue 2 has lower priority than in Queue 1.

Explanation :-
In this program we have to apply two tasks for a given number of processes.
Priority scheduling(Preemtive ):-
First task we have to do scheduling as per priority, and as mention it should be preemptive scheduling. First we ask the user to enter the number of processes he wants to schedule. After mentioning the number of processes , we have to enter the following things:
1.Burst time of process
2.Arrival time of process 
3. Priority of that process
After user has entered the data then, see the process which has the least arrival time comparing to all the processes mentioned . This process will be executed first , if its burst time is more than the arrival time of next process , and it does not have priority less than the next process then current process will be pre-empted by the next process and it will be executed ,previous process will be sent to waiting state, with the reduced burst time(because it has been executed for some time ). Then the processes left (still to be executed ) in ready state will be executed according to their priority, processes in waiting state will be executed by comparing their priority with the processes in ready state.
If there is a scenario where the process with least arrival time has burst time less than the arrival time of next process then it will be executed totally and rest of the processes are executed according their priority.
Priority scheduling sometimes leads to starvation.
Round Robin Scheduling:-
Second task we have to do scheduling as per round robin, all the processes are executed according to the given time quantum ,first the process with least arrival time is executed for the mentioned time quantum, then it is put in waiting state and next process in ready state is executed. This whole procedure is continued until all the process have been executed.
Round robin scheduling gives all the processes a fair share of CPU processing.

