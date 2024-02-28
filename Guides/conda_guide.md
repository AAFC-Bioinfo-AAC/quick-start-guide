# Conda - An AAFC Code Catalogue Guide

## Table of contents

[[_TOC_]]

## Introduction to Conda

This is a summary page for basic usage of Conda. For more details or more advanced commands, please refer to the [Conda user guide](https://conda.io/projects/conda/en/latest/user-guide/index.html)

**Part of this document was taken from the [Biocluster documentation](https://redmine.biodiversity.agr.gc.ca/projects/biocluster/wiki/Installing_Conda) and [AAFC training documentation](https://gccode.ssc-spc.gc.ca/bioinformatics_aafc/training_documentation/linux_resources).**

### What is Conda?

Conda is an open source package and environment manager. It provides an easy way for users to install packages in isolated environments without worring about conflicting requirements.

### Why use Conda?

- Conda can be installed by any user into their own userspace (**you don't need admin rights**). This provides maximum control to users over their Conda installation.
- You can quickly install any version of a software without worrying about conflicts between your software's and/or other users' configurations
- You can have multiple environments, one for each of your projects or pipelines.
- You can easily export and import Conda environments from other users to replicate environments.

## Installation
If Conda is not already installed on your device, you will first need to install it.

Conda can be installed on all platforms (Windows, macOS, Linux), but most bioinformatics and data analysis packages are only available on Linux and macOS. **If you have a Windows computer we recommend using the Windows Subsystem for Linux. See [WSL Installation Guide](/WSL_Workshop/WSL_installation.md) for more info.** These instructions focus on the Linux installation of Miniconda but the process is almost identical for other platforms.

### 1. Download and run the install script

   Open a Linux terminal and enter the following command:

   ```bash
   wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
   sh Miniconda3-latest-Linux-x86_64.sh
   ```

### 2. Installation procedure

   You will be guided through a command line based installation wizard:

   1. Press `<Enter>` to continue.
   2. Press `q` to close the license or `<enter>` to scroll through it until you've read it all.
   3. Type `"yes"` to accept the license, then press `<enter>`.
   4. The default install location of `~/miniconda3/` is fine, so press `<enter>`.
   5. Running `conda init` is no longer the recommended way to enable Conda, so type `"no"` and press `<enter>`.

### 3. Enable the `conda` command

   At this point, Conda is installed in your home directory, but if you try running it now, you'll get an error. This is because you have not told the command line interpreter that you want Conda enabled in your path. You can do this by running the following command:

   ```bash
   source ~/miniconda3/etc/profile.d/conda.sh
   ```

   This command allows the command line interpreter to recognize Conda. You will likely want to run this command every time you connect to a Linux terminal (WSL, Biocluster, etc.), so you are encouraged to edit your ~/.bashrc file, and add that command to the end of the file.

### 4. Activate The Base environment

  Activate the base Conda environment by typing:   

   ```bash
   conda activate
   ```

   Your shell prompt will then become prepended with "(base)".   
   **This is how Conda tells you which environment is currently active.**

### 5. Configure Conda

   Conda comes mostly pre-configured, but there are some minor changes we recommend for bioinformatics users. We recommend adding the conda-forge and bioconda channels to your configuration. These channels are free community initiatives which follow a set of guidelines that ensure that the software packages are secure and usable. The conda-forge channel provides more general purpose software tools and libraries, while the bioconda channel focuses on bioinformatics software. To add these channels, run the following commands:

   ```bash
   conda config --add channels bioconda
   conda config --add channels conda-forge
   ```


### 6. Update Conda

Once you've installed Conda, you should ensure that it is up to the latest version. You can do this by running:

```bash
conda update conda
```
You are now all set to start using Conda.

## Usage
### Terms and definition

Conda has a simple syntax. There is only a short list of commands to know for basic Conda users. Before getting to the list of commands, here is a terminology table of the most common terms used with `conda`:

| Term | Definition |
| --- | --- |
| Conda package | An [archive](https://en.wikipedia.org/wiki/Archive_file) containing all of the executable files and configuration files necessary for a specific software tool or library, as well as metadata about the external dependencies of that software |
| Conda Environment | A directory into which Conda packages can be installed |
| Install | When a Conda package is installed, it is downloaded from Conda's online package repository, and unpacked into a given Conda environment |
| Activate | When a Conda environment is activated, it means that Conda has modified the user's system environment in such a way that the software and libraries in the Conda environment are now accessible to the user |
| Base Environment | The default Conda environment that is created when Conda is installed. It should initially only contain the Conda package and its dependencies. __Installing packages directly into the base environment is not recommended__ |
| Conda Channels | Different users who upload conda packages to the [Anaconda Cloud](https://anaconda.org/). Some of these channels are actually communities of users who collaborate on packaging software |


### Managing the Conda environment

Conda environments are used to isolate and manage multiple softwares/versions/dependencies that differ from project to project. Here is a list of basic commands to manage your Conda environments.  

*Replace all [ ] with desired parameters.*
#### Create a new environment

```bash
conda create -n [ENV_NAME]
```

#### Activate an environment

```bash
conda activate [ENV_NAME]
```

#### Deactivate current environment

```bash
conda deactivate
```


#### List available environments

```bash
conda env list
```

#### Remove an environment

```bash
conda deactivate
conda env remove -n [ENV_NAME]
```
#### Import an environment

Import an environment from a `.yml` file with the following command:

```bash
conda env create --file [ENV_NAME].yml
```

### Manage Conda Packages


#### Find a package

To find a package, either use the search bar on [anaconda.org](https://anaconda.org/) or google `conda <your package name>` and the first result should be the page of the package on [anaconda.org](https://anaconda.org/). The Anaconda search tool requires the exact name of the package, so **we recommend searching for the package on Google**. 
#### Install a package

Install the default version of a package in your active environment

```bash
conda install [PACKAGE_NAME]
```

Install a specific version of a package in your active environment

```bash
conda install [PACKAGE_NAME]=2.4.3
```

#### List installed packages

For the active environment

```bash
conda list
```

#### Update a package

```bash
conda update [PACKAGE_NAME]
```


#### Remove a package

```bash
conda remove [PACKAGE_NAME]
```

### Exporting a Conda environment

The best way to export a conda environmnet is using a YAML file. You can create the `.yml` file of your active environment with the following command:

```bash
# yml file with all packages dependencies and versions
conda env export > [ENV_NAME].yml
```

## Tips and best practices

  - Do not install all your packages in your base environment
  - Create one environment for each pipeline/projects

## Known Issues

### Conda HTTP error

Some AAFC users encountered an error after the installation of Conda on WSL. The error title is **CondaHTTPError: HTTP 000 CONECTION FAILED**. If this happen to you, simply run the installation script a second time with the `-u` argument to force a new install.

```bash
sh Miniconda3-latest-Linux-x86_64.sh -u
```

## Useful Links
 - [anaconda.org](https://anaconda.org/)
 - [Conda user guide](https://conda.io/projects/conda/en/latest/user-guide/index.html)


