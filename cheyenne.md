# Cheyenne Cheatsheet
Cheatsheet of commands to use for submitting and managing jobs on the NCAR CISL Cheyenne supercomputer sourced from NCAR CISL. 
Source: https://www2.cisl.ucar.edu/resources/computational-systems/cheyenne

## SUBMITTING JOBS

| Key/Command | Description |
| ----------- | ----------- |
| ``qsub <PBS Script Name>`` | Submit batch job |
| ``qcmd -- ./case.build`` | Default setting for resource intensive jobs that are non-interactive |
| ``qcmd -l walltime=12:00:00 -- ./case.build`` | Example of customized settings for resource intensive jobs that are non-interactive |
| ``qsub -I -l select=1:ncpus=36:mpiprocs=36 -l walltime=01:00:00 -q regular -A project_code`` | Example of starting an interactive job |
| ``qinteractive`` | Alternative to start interactive job using 1-hour |
| ``qinteractive -l select=2:ncpus=10:mpiprocs=10`` | Example of customized qinteractive |

## CHECKING AND MANAGING JOBS

| Key/Command | Description |
| ----------- | ----------- |
| ``qdel jobID`` | Kill pending or running job |
| ``qdel `qselect` `` | Kill all pending or running jobs |
| ``qhist -u $USER`` |  Information on finished jobs |
| ``qhist -u $USER -d N`` | Information on finished jobs with number of days specified |
| ``qhist -u $USER -f`` | List jobs with non-zero exit code (failed jobs) |
| ``qpeek jobID`` |  Examine the stdout log for job that is running |
| ``qpeek --error jobID`` | Examine the stderr log for job that is running |

## CHECKING AND MANAGING JOBS (USE SPARINGLY)

| Key/Command | Description |
| ----------- | ----------- |
| ``qstat`` | Status of all unfinished jobs (self) |
| ``qstat -u $USER`` | Status of all unfinished jobs (self) |
| ``qstat -f jobID`` | Status of specific job |
| ``qstat -x jobID`` | Status of specific job |
| ``qstat -q queue_name`` | Status of unfinished jobs by queue type |
| ``qstat -Q`` | List number of jobs by queue type |
| ``qstat -xwu $USER`` | Status of all pending, running, and finished jobs |


