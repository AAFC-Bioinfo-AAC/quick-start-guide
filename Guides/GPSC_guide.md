# Working with the GPSC
> Note:
    You must first have access to the GPSC. To request an account, follow the instructions found [here](https://gcxgce.sharepoint.com/teams/1000645/SitePages/GPSC-Guides.aspx?OR=Teams-HL&CT=1708971900190&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiIyNy8yNDAxMDQxNzUwNCIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D#fill-out-account-request-form).  

[[_TOC_]]

## What is the GPSC
The [General Purpose Science Cluster (GPSC)](https://portal.science.gc.ca/confluence/) is a High-Performance Computer (HPC) provided by Shared Service Canada (SSC). All code catalogue pipelines are compatible for use on the GPSC. A [complete list of computing resources](https://portal.science.gc.ca/confluence/display/SCIDOCS/Compute+Resources) can be found in the SSC guide.

## GPSC Locations
>*replace with table comparing three?*
### 1. Interactive containers
Interactive containers have full access to the internet and can be used to:
- download **small to moderate** amounts of data
- **install** software
- set up a new **Conda** environments.

### 2. Compute clusters
Compute clusters should mainly be **used for analysis**. Jobs running on the clusters have limited access to the internet, so it’s best to first download data from an interactive container or landing pad and *then* run your analysis on a compute cluster.

### 3. Landing pads
The landing pad is used to initially connect to the GPSC, before connecting to an interactive container and should not be used for HPC workloads, but can be used to download data before running an analysis.  

If you need to download large amounts of data you can do this on the following landing pad:

    inter-aafc-lp.science.gc.ca

> Note: Space on the GPSC is limited. When downloading files or running an analysis, please make sure to not do so on your home directory, as it can only hold 10Gb of material, and make sure to move files that don't need to be on the GPSC to another location.

## Connecting to the GPSC
There are many different ways to connect to the GPSC. A list of connection methods can be found [here](https://gcxgce.sharepoint.com/teams/1000645/SitePages/GPSC-Guides.aspx?OR=Teams-HL&CT=1708971900190&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiIyNy8yNDAxMDQxNzUwNCIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D#connecting-to-the-gpsc).  


## Using the GPSC

### Interactive jobs
Interactive jobs are similar to running an analysis on your local computer and require interaction from the user. They:
- should be used for shorter jobs or troubleshooting scripts.
- must remain connected to the GPSC throughout the job.
- do not require job submission files.
- should **avoid** heavy computational work.

To log in to an interactive container, enter from the landing pad:

    $ ssh inter-aafc-ubuntu2204.science.gc.ca

You can now run the required commands in an interactive session.

Run the `exit` command when you have completed your work and are ready to exit the container. This will bring you back to the landing pad which you can exit as well.


### Batch jobs
Batch jobs allow the user to submit a job and walk away while it is being run. They:
- can be used for short or long running jobs (minutes to weeks).
- require a job submission file containing the relevant commands.
- do not need user interaction.

The GPSC uses [SLURM](https://slurm.schedmd.com/documentation.html) to manage and submit job.  

To **submit** a job use the `sbatch` command:  
    
    $ sbatch [file_name].sh

Additional information on commands are available on the [SSC site](https://portal.science.gc.ca/confluence/display/SCIDOCS/Quick+Start+to+Using+Linux+Clusters+With+SLURM).

### Array jobs 
Job arrays allow the user to submit a collection of similar jobs at the same time, allowing them to be run more quickly. They are submitted similarly to batch jobs, so all the jobs must have the same submission options. When using the `sbatch` command to submit a job, the `--array=0-[number_of_jobs]` option should be added to indicate an array of jobs will be submitted instead of a single batch job. 

You should also indicate the output and error file names using the `--output=[name]_%A_%a.out` and `--error=[name]_%A_%a.err`.  
In these commands:
- `%A` corresponds to the array's job ID.
- `%a` corresponds to the job's array index value.  

More indepth information can be found [here](https://slurm.schedmd.com/job_array.html).

### GPU usage
Jobs on the GPSC can be run using CPUs or GPUs. GPUs excel in handling parallel computations compared to CPUs. For some tools to run optimally, they should request GPU usage when submitted. To do this, when submitting a SLURM job, users can use the `--gres=gpu:[number_of_gpus]` or `--gpus-per-task=[number_of_gpus]` options along with the `gpu_a100` partition. Not all GPSC clusters have access to GPUs. If you wish to incorporate them into your workflow, please ensure you use the `gpsc7` cluster. It is equipped with 48 NVIDIA DGX A100s in total, 8 per compute core. More information on the gpsc7 cluster's resources can be found [here](https://portal.science.gc.ca/confluence/display/SCIDOCS/gpsc7).

## Common Resources available on the GPSC
    TBD

## Adapting pipelines to run on the GPSC
### How to adapt a bash script 

### How to adapt snakemake script

### How to adapt nextflow script



