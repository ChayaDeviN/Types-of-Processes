# Types-of-Processes
Depicts various types of processes involved in a parent-child interaction process


ZOMBIE PROCESS

A process which has finished the execution but still has entry in the process table to report to its parent process is known as a zombie process. A child process always first becomes a zombie before being removed from the process table. The parent process reads the exit status of the child process which reaps off the child process entry from the process table.

The different states of a zombie process can be observed using the command:

ps -l



ORPHAN PROCESS

A process whose parent process no more exists i.e. either finished or terminated without waiting for its child process to terminate is called an orphan process.

DAEMON PROCESS


A Daemon process is a process which is not associated with any terminal and hence is supposed to run in background. Since, a daemon process involves background processing, it is recommended it should not include any user interaction. Therefore, it should be clear about its continuous processing not caring to wait for any input or to display any output. However, C programming does not define any such restrictions in its development as such. A daemon process developer should be well aware of its definition and ideal functionality before one starts the programming.


The daemon process running in the background can be checked using :

ps -A|grep "daemon"
