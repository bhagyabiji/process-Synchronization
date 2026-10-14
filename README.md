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
