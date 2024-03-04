# A Short GPSC Guide
> Note:
    You must first have access to the GPSC. To request an account, follow the instructions found [here](https://gcxgce.sharepoint.com/teams/1000645/SitePages/GPSC-Guides.aspx?OR=Teams-HL&CT=1708971900190&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiIyNy8yNDAxMDQxNzUwNCIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D#fill-out-account-request-form).  

[[_TOC_]]

## What is the GPSC
The [General Purpose Science Cluster (GPSC)](https://portal.science.gc.ca/confluence/) is a High-Performance Computer (HPC) provided by Shared Service Canada (SSC). As a member of the Code Catalogue, you will primarily be working on __, but a [complete list of computing resources](https://portal.science.gc.ca/confluence/display/SCIDOCS/Compute+Resources) can be found in the SSC guide.

## GPSC Locations
### 1. Interactive containers
Interactive containers have full access to the internet and can be used to download small to moderate amounts of data, install software, and set up a new Conda environments.

### 2. Compute clusters
Compute clusters should mainly be used for analysis. Jobs running on the clusters have limited access to the internet, so it’s best to first download data from an interactive container or landing pad and *then* run your analysis on a compute cluster.

### 3. Landing pads
The landing pad is used to initially connect to the GPSC, before connecting to an interactive container and should not be used for HPC workloads, but can be used to download data before running an analysis..  

If you need to download large amounts of data you can do this on the following landing pad:

    inter-[dept.]-lp.science.gc.ca

## Connecting to the GPSC
There are many different ways to connect to the GPSC. This guide will explain how to connect through VS Code, which we recommend for less experienced users, but a larger list of connection methods can be found [here](https://gcxgce.sharepoint.com/teams/1000645/SitePages/GPSC-Guides.aspx?OR=Teams-HL&CT=1708971900190&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiIyNy8yNDAxMDQxNzUwNCIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D#connecting-to-the-gpsc).  

### Prerequisites
- You must either be on an operating system that already has SSH pre-installed or you will have to install an [OpenSSH compatible SSH client](https://code.visualstudio.com/docs/remote/troubleshooting#_installing-a-supported-ssh-client).  
    > You can check if SSH is already installed on your machine by typing `ssh` into your terminal. If it is not installed it will indicate that it does not know that command.  
- [Install VS Code](https://code.visualstudio.com/).
- Install the [Remote-SSH extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh) in VS Code.
    > This can be done by searching for **Remote-SSH** in the **extensions** tab on the left-hand side of your VS Code window. Once it is installed you should see a `><` button in the bottom-left corner of your window. If you do not see it, try restarting VS Code.  

### Connecting to the GPSC Landing Pad
To connect to the GPSC using VS Code:
1. Open VS Code and click the `><` button in the bottom-left corner of your window.
2. Select “Connect to Host…” from the prompt.
3. Enter: `[your_username]@inter-[dept.]-lp-gccloud.science.gc.ca`
    >The first time you connect you will likely be asked if you want to continue. Select “yes” for all steps. You will also likely be asked what `platform` the remote host is. Select `Linux`.
4. Enter your GPSC password when requested.
This will connect you to the GPSC landing pad.  
    > Note: Unless you do the [optional step](#optional-set-up-vs-code-to-connect-automatically-to-the-gpsc) below you wil only be able to access the VScode text editor on the landing pad.
### Connecting to an Interactive Container
To connect to an interactive container:
1. Open a terminal in VS Code.
2. Enter:
    $ ssh inter-[dept.]-ubuntu2204.science.gc.ca
3. Enter your password when prompted.  

**Congratulations**, you are now in an interactive container! From here you can use the GPSC’s resources on VS Code.

### OPTIONAL: Set up VS Code to connect automatically to the GPSC. 
Steps on how to do this can be found [here](https://gcxgce.sharepoint.com/teams/1000645/SitePages/GPSC-Guides.aspx?OR=Teams-HL&CT=1708971900190&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiIyNy8yNDAxMDQxNzUwNCIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D#connecting-to-the-gpsc).

## Using the GPSC
### Scheduling
The GPSC uses fairshare scheduling to prioritize jobs based on:  
- project allocation on the GPSC.  
- past usage.  

Thus, scheduling priority is dynamically determined and may fluctuate depending on allocations, usage, and other job requests. Projects have predetermined allocations on the GPSC, so it is important to include your specific project tag in your job submission. Jobs submitted on clusters without partner allocations have the lowest priority. 

The goal is to trend towards ‘fairness’ over time. This does not guarantee usage at any specific point in time.  

### Interactive jobs
Interactive jobs are similar to running an analysis on your local computer and require interaction from the user. They:
- should be used for shorter jobs or troubleshooting scripts.
- must remain connected to the GPSC throughout the job.
- do not require job submission files.
- should **avoid** heavy computational work.

To log in to an interactive container, ssh to inter-[dept.]-ubuntu2204.science.gc.ca from the landing pad.

    $ ssh inter-[dept.]-ubuntu2204.science.gc.ca

You can now run the required commands in an interactive session.

Run the exit command when you have completed your work and are ready to exit the container. This will bring you back to the GCCloud landing pad which you can exit as well.

    $ exit
    logout
    Connection to inter-[dept.]-ubuntu2204.science.gc.ca closed.
    $ exit   
    logout
    Connection to inter-[dept.]-lp-gccloud.science.gc.ca closed.

### Batch jobs
Batch jobs allow the user to submit a job and walk away while it is being run. They:
- can be used for short or long running jobs (minutes to weeks).
- require a job submission file containing the relevant commands.
- do not need user interaction.

The GPSC uses [SLURM](https://slurm.schedmd.com/documentation.html) to manage and submit job.  

To **submit** a job use the `sbatch` command:  
    
    $ sbatch [file_name].sh

To check the **status** of your job use the `squeue` command:  
   
    $ squeue -u <username>  
When the job disappears from the returned list, it is finished.

Additional information on using sbatch and squeue is available on the [SSC site](https://portal.science.gc.ca/confluence/display/SCIDOCS/Quick+Start+to+Using+Linux+Clusters+With+SLURM).

## FAQs
### How do I check my group membership?

    $ id [user_id]

### Which department acronyms have access to the GPSC?
- aafc
- cfia
- dfo
- eccc
- hc
- nrc
- nrcan
- phac

### How can I change my password?

    $ passwd
    [Enter old password]
    [Enter new password]

