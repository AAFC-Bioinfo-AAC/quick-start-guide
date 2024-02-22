# AAFC Pipeline Creation Guide
[[_TOC_]] 



## Creating a Pipeline
### Before Starting
The AAFC Code Catalogue is __ . Before creating a pipeline, make sure that you take a look at the pipelines that have already been created or are in development and are familiar with the pipeline [requirements](pipeline_guidelines.md) and [git basics](LINK).  

Once you have an idea for a workflow you'd like to contribute to the Code Catalogue, submit a [pipeline proposal form](LINK) to confirm that it does not overlap with other pipelines that are in development or that have been suggested. This form will be reviewed by a member of the Code Catalogue team, who will confirm the uniqueness of your proposed pipeline. If it is too similar, consider contributing to the already existing pipeline or collaborating with others who have suggested a similar project. A core team member will be able to put you in contact with the persons in question.  

### Copy the template
>*If we can have a template repo on github, we can remove steps 9 to 11*

A repository is only added to the Code Catalogue once it is ready to be deployed. This is to ensure that the catalogue is not filled with copies of the template project when a pipeline's development takes longer than expected. 

To begin, login to your GitLab account and create a local project repository by forking the [pipeline template](LINK):  

1. Go to the [pipeline template](LINK)'s repository, and click on the `Fork` button in the upper-right corner of the page.  
> INSERT IMAGE HERE
2. Edit the ***Project name***. This will be the working name of your pipeline. The name can be changed later, so do not worry if it's not finalized.
3. Under ***Project URL***, select the `namespace` your fork should belong to from the dropdown menu and add a `Project Slug`, which will be the end of the URL to your project.
4. ***Optional*** Add a Project description.
6. Select include `All branches`.
7. Select the Visibility level for your fork. (We should suggest one, don't know what the rules are with the government, assuming cannot be public.)
8. Click `Fork project` and you will be redirected to the newly created fork’s page.
9. On this new page, select `Settings > General` from the left sidebar.
> INSERT IMAGE HERE
10. Expand the `Advanced` section at the bottom of the page and select `Remove fork relationship`.
11. Enter the project path, and click `Confirm`.

> *add something about making a local clone?*

### Work on your pipeline  
Each project must fulfill the requirements outlined in the [pipeline guidelines](pipeline_guidelines.md).

> wait, does this make sense? what is being added to the catalogue? is it just a link of this pipeline directly or is it a new "official" copy? How can we manage versioning? Once ready to release the user would transfer ownership to the code catalogue account? (that's how nf-core does it right now. Then they can still collaborate but need approved pull requests to publish to main)

- Switch to the `dev` branch of the repository. 
    > $ git checkout dev  

    All development should happen on `dev` branch or be merged into the `dev` branch and kept away from `main`. 
- [Create a conda environment](LINK) for your project and install any tools you may need.
- You can begin coding your pipeline as usual using standard git development workflow in the `workflow` folder. If you already have a pipeline created, you can instead import its files directly into the `workflow` folder.  
- Test your workflow to ensure it produces consistent and reproducible results. If you do not have your own test data, minimal datasets are available at [__](LINK).  
- Once complete, fill out the `LICENSE`, `README.md`, `CITATIONS.md`, `CITATION.cff`, and `CHANGELOG.md` files as specified in [_](LINK).
- [Export your conda environment](LINK) and place it in the `config` folder.

[REPOSITORY PATH]
    ├── config
    │   ├── env_[PIPELINE NAME].yml
    |   └── ...
    ├── workflow
    │   ├── ...
    │   └── ...
    ├── LICENSE
    ├── README.md
    ├── CITATIONS.md
    ├── CITATION.cff
    ├── CHANGELOG.md
    └── .gitignore

    


## Adding your Pipeline to the Code Catalogue

## Updating your Pipeline