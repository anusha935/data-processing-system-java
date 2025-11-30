Data Processing System – Java Version

This section explains how the Java implementation of the Data Processing System was run and verified.

Requirements

Online Java compiler such as Online Java Compiler.

Java JDK 8 or later (if running locally).

Steps to Run

Open the online Java compiler in your browser.

Write the complete Java code for Main.java in the editor, including:

Main class

Worker class

TaskQueue class (if used)

Click Run / Execute. The program compiles and starts executing.

The program creates output files for each worker:

Worker-1_output.txt

Worker-2_output.txt

Worker-3_output.txt

Check the console logs for the following outputs, showing concurrent task processing:

Nov 30 11:26:59 AM System Started.
Nov 30 11:26:59 AM Worker-1 started.
Nov 30 11:26:59 AM Worker-2 started.
Nov 30 11:26:59 AM Worker-3 started.
Nov 30 11:27:00 AM Worker-1 processed Task 1
Nov 30 11:27:00 AM Worker-2 processed Task 2
Nov 30 11:27:00 AM Worker-3 processed Task 3
...
Nov 30 11:27:01 AM Worker-3 finished.
Nov 30 11:27:01 AM System completed all tasks.

Notes

Output files were successfully created in the same folder as the code, containing all tasks processed by each worker.

The number of workers and tasks can be changed in main by modifying numWorkers and numTasks.

Thread synchronization ensures no data is missed or duplicated.
