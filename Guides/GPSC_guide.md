# A Short GPSC Guide
> Note:
    You must first have access to the GPSC. To request an account, follow the instructions [here](https://gcxgce.sharepoint.com/teams/1000645/SitePages/GPSC-Guides.aspx?OR=Teams-HL&CT=1708971900190&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiIyNy8yNDAxMDQxNzUwNCIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D#fill-out-account-request-form)  

## What is the GPSC
The [General Purpose Science Cluster (GPSC)](https://portal.science.gc.ca/confluence/) is a High-Performance Computer (HPC) provided by Shared Service Canada (SSC). As a member of the Code Catalogue, you will primarily be working on __, but a [complete list of computing resources](https://portal.science.gc.ca/confluence/display/SCIDOCS/Compute+Resources)) can be found in the SSC guide.

## Connecting to the GPSC


## GPSC Locations
### 1. Interactive containers
Interactive containers have full access to the internet and can be used to download small to moderate amounts of data, install software, and set up a new Conda environments.

### 2. Compute clusters
Compute clusters should mainly be used for analysis. Jobs running on the clusters have limited access to the internet, so it’s best to first download data from an interactive container or landing pad and *then* run your analysis on a compute cluster.

### 3. Landing pads
The landing pad is used to initially connect to the GPSC, before connecting to an interactive container and should not be used for HPC workloads, but can be used to download data before running an analysis..  

If you need to download large amounts of data you can do this on the following landing pad:

    inter-<dept>-lp.science.gc.ca

## Using the GPSC
0. GPSC fairshare scheduling
Fairshare scheduling is used to prioritize jobs based on:

allocation on the GPSC as determined by agreement between the project (GRDI) and SSC
past usage
The goal is to trend towards ‘fairness’ over time. This does not guarantee usage at any specific point in time.

0.1. Scheduling priority
Scheduling priority:

is dynamically determined
may fluctuate depending on allocations, usage, and other job requests
e.g.: a job submitted under a project with low accumulated usage may jump ahead of other jobs already waiting
0.2. Project tags
grdi_genarcc is the code specific to the GenARCC project.
Use of tags in jobs is very important for tracking usage against project GPSC allocation.
Jobs submitted on clusters without partner allocations have the lowest priority.
Analysis jobs can be run on the GPSC in two different ways, as interactive jobs or batch jobs.

### Interactive jobs
Interactive jobs are similar to running an analysis on your local computer and require interaction from the user. They:
- should be used for shorter jobs or troubleshooting scripts.
- must remain connected to the GPSC throughout the job.
- do not require job submission files.
- should **avoid** heavy computational work.

To log in to an interactive container, ssh to inter-<dept>-ubuntu2204.science.gc.ca from the landing pad.

    $ ssh inter-aafc-ubuntu2204.science.gc.ca

You can now run the required commands in an interactive session.

Run the exit command when you have completed your work and are ready to exit the container. This will bring you back to the GCCloud landing pad which you can exit as well.

    $ exit
    logout
    Connection to inter-aafc-ubuntu2204.science.gc.ca closed.
    $ exit   
    logout
    Connection to inter-aafc-lp-gccloud.science.gc.ca closed.

### Batch jobs
Batch jobs allow the user to submit a job and walk away while it is being run. They:
- can be used for short or long running jobs (minutes to weeks).
- require a job submission file containing the relevant commands.
- do not need user interaction.

2.1. Sample batch job file (hello_sleeper.sh)
#!/bin/bash -l
#SBATCH --job-name=sleeper
#SBATCH --output=sleep.out
#SBATCH --partition=standard
#SBATCH --account=grdi_genarcc
#SBATCH --time=00:00:60
#SBATCH --ntasks=1
#SBATCH --cpus-per-task=1
#SBATCH --mem-per-cpu=2000M
#SBATCH --comment="registry.maze.science.gc.ca/ssc-hpcs/generic-job:ubuntu22.04"
 
echo hello
sleep 60
echo goodbye

2.2. Commands
2.2.1. Submit job: sbatch
To submit the job displayed above, named hello_sleeper.sh, type:

sbatch hello_sleeper.sh

2.2.2. Monitor job status: squeue jobst
To monitor the status of your jobs, type:

$ squeue -u <username>

Sample output:

meb000@inter-aafc-ubuntu2204:~/tutorials/intro_gpsc$ sbatch sleeper.sh
Submitted batch job 42961
meb000@inter-aafc-ubuntu2204:~/tutorials/intro_gpsc$ squeue -u meb000
             JOBID PARTITION     NAME     USER ST       TIME  NODES NODELIST(REASON)
             42961  standard  sleeper   meb000  R       0:13      1 ib14be-021
When the job disappears from the list, it is finished.

Additional information on using sbatch and squeue is available in the .




