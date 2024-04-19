## Introduction to Apptainter (formerly Singularity)
[[_TOC_]]
### What is Apptainer?
Apptainer, formerly known as Singularity, is a containerization program specifically designed for scientific and high-performance computing. It allows users to pack the entirety of their working environment into "containers" that can be run anywhere. These containers simulate that working environment ensuring secure, reliable, and reproducable analysis. 
### Why use Apptainer?
Apptainer works with your computer's host to encapsulate complex software environments. This means your jobs will be able to run in a consistent environment that is easily reproducible by others. By eliminating software compatibility issues, Apptainer containers:
- improve the flexibility of computing resources.
- ensure reproducible analysis.
- extend the life of existing resources and depreceated tools.
- facilitate collaboration between researchers. 
## Installation
To create containers or run containers locally, you will need to have a local version of Apptainer installed. The apptainer software is only able to run on linux, but Windows users can install it using a [Windows Subsystem for Linux (WSL)](https://ubuntu.com/desktop/wsl). Other Mac and Windows installation options can be found [here](https://apptainer.org/docs/admin/main/installation.html#installation-on-windows-or-mac).  

[Install version 1.2.1](https://github.com/apptainer/apptainer/blob/release-1.2/INSTALL.md) of Apptainer from source.

## Usage
### Definition Files
Apptainer uses definition files (.def) as instructions to build custom containers. They contain specifics about:
- which Operating System to use
- what software to install 
- what metadata to include
- what environment variables to set at runtime
- which files to add from the host system 

Apptainer definition files are divided into two parts:
- [***Headers***](https://apptainer.org/docs/user/main/definition_files.html#header): *Mandatory*. Describes the core operating system of the container. It contains the desired bootstrap agent to be used and other information associated with that agent.
    > bootstrap: [<*desired bootstrap agent*>](https://apptainer.org/docs/user/main/appendix.html#buildmodules)  
     

- ***Sections***: *Optional*. Each section is defined by a % character and the section name. They provide additional information or instructions for the creation of the container.    

     - **%label**: used to define metadata. Can be viewed using `apptainer inspect [container_name].sif`
        *Example:*
        >    %labels  
                Author [Name]  
                Maintainer [email]  
                URL [website]  
 
    - **%files**: indicates where to copy specific files from the host system into the container system. 
        *Example:*
        > %files  
            [file path to be copied] [location to place copy]
           
    - **%environment**: defines the container's environment variables at runtime. Can be used to set up communication or file passing between the container and outside environment. These variables are only available at runtime.
        *Example:*
        > %environment  
        export PATH="$PATH:/opt"

     - **%post**: customizes the building process of your container. Usually used to update and install software.  
        *Example:*
        > %post  
            echo "Installing required packages..."  
            apt-get update && apt-get -y upgrade  
            apt-get install -y [software]
            mkdir ./output  
    - **%test**: validates the container after the building process is complete by comparing it to a specific output file.  
        *Example:* 
        >%test  
            [output].out  
    - **%runscript**: contains a list of default commands that will execute when the container is `run`.  
        *Example:* 
        >%runscript  
            echo "The output of your program is:"  
            /opt/output.out
    - **%help**: contains the text that will displayed if the `help` command is used.  
        *Example:*
        > %help  
        To run the container:
	`apptainer run <container_name.sif>`  
    To shell into the container:
	`apptainer shell <container_name.sif>`  
    To execute a custom command or app:
	`apptainer exec <container_name.sif> <command or app_name>`  
    To view the container's metadata:
	`apptainer inspect <container_name.sif>`  

### Creating a container
1. Make sure you have installed *Apptainer* locally and have `sudo` access on your machine. 
2. Create a definition file for your desired container configuration. We suggest naming it [name_of_your_pipeline].def
3. Build the container:  
    >$ apptainer build [desired_container_name].sif [definition_file_name].def
### Using a container  
There are two main ways you will be using your container, as a **shell** , as a **script** itself or to **execute** another script. Containers can also be used in conjunction with **SLURM**.

#### Shell
Using the container as a shell will allow you to work within the container from the command line as if it were your own native OS. This can be done using the `shell` command:  

    $ apptainer shell [container_name].sif

The following at the beginning of your terminal line will indicate that you are inside the shell:

    Apptainer> 

#### Script
If a `%runscript` section was included in the definition file that the container was created from, then the container will be able to be run as a script. The `run` command will execute the commands in the runscript section.  

    $ apptainer run [container_name].sif  

The container can also be run directly as an executable:
	./[container_name].sif


#### Execute another script
When executing any normal script, it can also be specified to run using a specific container using the `exec` command:
    
    apptainer exec [container_name].sif [script_to_run]  

#### Batch jobs
The same container commands can be included in SLURM job submissions by creating a regular job script:  

    #!/bin/bash

    #SBATCH --job-name=test_container
    #SBATCH --output=test_container-%j.out
    #SBATCH --ntasks=1
    #SBATCH --cpus-per-task=1
    #SBATCH --mem-per-cpu=5G
    #SBATCH -p normal
    #SBATCH --time 00:10:00

    apptainer run [container_name].sif

## Example  

*TBD*