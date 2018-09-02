# job-scheduler

Initially a set of job is given with its job_id, arrival_time (which will be 0) and execution_time. There
is a single processor which can be used to execute these jobs. Each job will get a fixed amount of time
(say d) to execute in the processor. Once that time duration is over then the next job will get the chance
to execute and the current job, if it is not yet completed, will go to the end of the job queue. This job
switching time is considered to be negligible. New jobs may also arrive after the job scheduling process
is started. In that case the arrival_time is assumed to be greater than 0. Once a new job arrives; it will be
added to the job queue. If at any point of time, a new job arrives and also an existing job completed its
‘d’ amount of time in the processor, then first the new job will be added to the job queue and then the
existing job will be added to the job queue. Perform the job scheduling and show the status of job
scheduling after a certain time instant. Display each job with job_id, arrival_time, execution_time,
start_time, finish_time, remaining_time, status (Completed or Not completed).

Example: 
Enter processor allotted time d: 5
Enter the initial set of jobs at time = 0
No. of jobs: 5
&lt;Job_Id, Arrival_time, Execution_time&gt;
JId1 0 18
JId2 0 4
JId3 0 7
JId4 0 9
JId5 0 6
Any more jobs at later time: Yes
No. of jobs: 1
&lt;Job_Id, Arrival_time, Execution_time&gt;
JId6 18 20
Any more jobs at later time: No
Enter the time instant for displaying the job scheduling result: 10

Job Scheduling Status at time instant 10.

![alt text](https://github.com/cozek/job-scheduler/raw/master/sample_output.JPG)
