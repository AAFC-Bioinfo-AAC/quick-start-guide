## Introduction to Apptainter (formerly Singularity)
### What is Apptainer?
### Why use Apptainer?
## Installation
To create containers or run containers locally, you will need to have a local version of Apptainer installed. The apptainer software is only able to run on linux, but Windows users can install it using a [Windows Subsystem for Linux (WSL)](LINK). Other Mac and Windows installation options can be found [here](https://apptainer.org/docs/admin/main/installation.html#installation-on-windows-or-mac).  

Install version 1.2.1 for use on the GPSC.
> Insert installation steps here...

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
           
    - **%environment**: defines the container's environment variables at runtime. These variables are only available at runtime.
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
    > Note:  
    If you will be using your container on the GPSC, consider using one of the [provided containers](https://portal.science.gc.ca/confluence/display/PSGRDI/gpsc7#:~:text=InteloneAPI%2D2022.1.2%2DTorunMPIprograms-,Job%20Submission,-The%20queueing%20system) as your starting point.
3. Build the container:  
    >$ apptainer build [desired_container_name].sif [definition_file_name].def
### Using a container  