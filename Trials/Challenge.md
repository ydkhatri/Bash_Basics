# Challenge Assignment

Write a bash script (.sh) to collect :

- all executable files that are above 512000 bytes (~500KB) and below 30720000 (~30MB) in size
- all TXT files created or modified within the last 15 days
- all log files that are over 65536 bytes (~64KB)

Collect the files and also the following information about them (we shall call this **R1**)
Name, Size, Full Path, SHA1 hash, MAC times, Owner

Your script should keep a record of the statistics (we'll call this **R2**) , ie,

- Total files scanned.
- Total number of executable files, TXT, log files.
- Total number of executable files, TXT, log files responsive (to be collected)

You will then run your script on the entire root drive of your lab machine and document the results.

**R3**: You must use reasonable measures to ensure the collection is complete and accurate. You will document the script run, Also provide a list of all paths that were inaccessible by the script (that it failed to scan) and any files that it failed to collect. Write about how one would get those files too. You don't need to implement it, but provide an explanation.

**R4**: Summarize the statistics in a table. How many total files? How many files were found in system locations (/etc/) vs User locations (/home/)?

Your submission will be a short report explaining the task assigned to you, a screenshot of the code in action and the R2 statistics along with R3 & R4. R1 can be attached as a csv or excel sheet. Also provide your working code. The code must be commented to explain its working. The final collection of files should not be attached here.

You can consult the Tutors on this one and/or come to me with problems. But you must first spend some time to try to solve the issues on your own.
