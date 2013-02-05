*Percept2 -- A Concurrent Erlang Profiling Tool*

================================

`Percept2` is an enhanced version of the `Percept` (see  http://www.erlang.org/doc/man/percept.html) profiling tool from the Erlang/OTP distribution. 
 Percept2 extends Percept in both functionality and scalability. Among the new functionalities added are:
 
 * scheduler activity: the number of active schedulers at any time during the profiling;

 * process migration information: the migration history of a process between run queues;

 * statistics data about message passing between processes: the number of messages, and the average message size, sent/received by a process;

 * accumulated runtime per-process: the accumulated time when a process is in a running state;

 * process tree: the hierarchy structure indicating the parent-child relationships between processes;

 * dynamic calling-context-aware function call graph;
 
 * active functions: the functions that are active during a specific time interval, and

 * inter-node message passing: the sending of messages from one node to another.

 ### How to build Percept2 ###
 
 Build and install the software in the usual way:
 
 
       $ ./configure 
       
       $ make 
       
       $ (sudo) make install
  
   By default Percept2 is installed under the directory `/usr/local`;
   to install Percept2 in a different directory, you need to explicitly
   specify the directory using the '--prefix=...' flag of 'configure'.
 
   NOTE: percept2 uses the `graphviz' tool to generate the graph representation 
   of process tree and dynamic function callgraph. While we are trying to remove 
   this dependence, please make sure graphviz is installed on your machine for now.
   
### Documentation ###

 Percept2 online documentation is available from http://huiqing.github.com/percept2











