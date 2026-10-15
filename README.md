PROCESS SYNCHRONIZATION
-----------------------

- four types of solutions to the process synchronization problem −

  1. Locks
  2. Semaphores
  3. Monitors
  4. Interrupt Disable
     
- Critical Section
- Critical Section problem
       do {
            entry section      // ask permission
            critical section
            exit section       // release
            remainder section
  } while (true);

DEADLOCK 
--------
In an operating system, deadlock is a state in which two or more processes are unable to proceed because each is waiting for a resource that the other holds, resulting in a cycle of dependencies. 

Conditions for Deadlock
-----------------------
1. Mutual Exclusion 
− At least one resource must be held in a non-shareable mode, meaning only one process can use it at a time. Example: A printer can only be used by one process at a time.

2. Hold and Wait 
− A process holding at least one resource is waiting to acquire additional resources that are currently being held by other processes. Example: Process A holds a printer and waits for a scanner, while Process B holds a scanner and waits for the printer.

3. No Preemption 
− Resources cannot be forcibly taken away from processes holding them. A process must release the resource voluntarily when it is no longer needed. Example: If Process A is holding a printer and is waiting for a scanner, the system cannot force Process A to give up the printer.

4. Circular Wait 
− A set of processes exist such that each process in the set is waiting for a resource that another process in the set holds, forming a cycle of dependencies. Example: Process A waits for Process 's resource, Process B waits for Process 's resource, and Process C waits for Process 's resource, forming a circular chain.

