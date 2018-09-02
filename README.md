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
**Note: The input format varies slightly in the program in my repository.**
## Example: 

1. Enter processor allotted time d: 5
2. Enter the initial set of jobs at time = 0
3. No. of jobs: 5


Job id  | Arrival Time  | Execution Time | 
--------|-------------- |--------------- |
Job1    | 0             | 18             |
Job2    | 0             | 04             |
Job3    | 0             | 07             |
Job4    | 0             | 09             |
Job5    | 0             | 06             |


## Jobs that arrive later

Job id  | Arrival Time  | Execution Time | 
--------|-------------- |--------------- |
Job6    | 20             | 18             |



Enter the time instant for displaying the job scheduling result: 10


### Job Scheduling Status at time instant 10.

![alt text](https://github.com/cozek/job-scheduler/raw/master/sample_output.JPG)

