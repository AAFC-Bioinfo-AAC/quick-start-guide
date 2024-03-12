# How To Contribute
[[_TOC_]] 

## Before Starting
The AAFC Code Catalogue is [describe the role of the code catalogue] . If you have an idea for a workflow you'd like to contribute to the Code Catalogue, message [__](LINK) to be added to the Code Catalogue group. Once added, you'll be able to create a new project repository and publish to the catalogue. To facilitate this process, we've created a set of pipeline [recommendations](pipeline_guidelines.md#suggestions), a [project template](LINK), and [useful guides](README.md#guides).    

 Before creating a pipeline, we suggest taking a look at the pipelines that have already been created or are in development. If a pipeline that is very similar to yours already exists, consider collaborating on that pipeline instead of creating a new one. 

## Creating a Pipeline
There are two options for contributing a pipeline to the catalogue. You can either:  
- [Use the provided template to create a new pipeline from scratch](#from-the-template).
- [Upload a pipeline you have already created](#from-an-existing-project). 

### From the Template
#### 1. Copy the template 

To begin, login to your GitLab account and create a local project repository by forking the [pipeline template](LINK):  

1. Go to the [pipeline template](LINK)'s repository, and click on the `Fork` button in the upper-right corner of the page.  
2. Edit the ***Project name***. This will be the working name of your pipeline. The name can be changed later, so do not worry if it's not finalized.
3. Under ***Project URL***, select the `code_catalogue` namespace from the dropdown menu and add a `Project Slug`, which will be the end of the URL to your project. We recommend that it matches the name of your pipeline.
4. ***Optional*** Add a Project description.
6. Select include `All branches`.
7. Select `Private` as the visibility level. 
8. Click `Fork project` and you will be redirected to the newly created fork’s page.
9. On this new page, select `Settings > General` from the left sidebar.
10. Expand the `Advanced` section at the bottom of the page and select `Remove fork relationship`.
11. Enter the project path, and click `Confirm`.

A repository should be set to `private` until it is ready to be deployed. This is to ensure that the catalogue is not filled with copies of the empty template project if a pipeline's development takes longer than expected. Individuals who have been added to the Code Catalogue group will be able to see all project repositories, even those set to private. This will only prevent the *public* from having to sift through empty pipelines.  

#### 2. Work on your pipeline  
The template repository has two branches, `main` and `dev`. We suggest that all active development happens on the `dev` branch and that `main` only be used to house stable version releases of the pipeline.

Each project should fulfill the requirements outlined in the [pipeline guidelines](pipeline_guidelines.md#suggestions).

- Switch to the `dev` branch of the repository. 
    > $ git checkout dev  
- [Create a conda environment](conda_guide.md#create-a-new-environment) for your project and [install](conda_guide.md#manage-conda-packages) any tools you need as you go.
- You can begin coding your pipeline as usual using standard git development workflow. If you already have a pipeline created, you can instead import its files directly. We suggest placing your code in the `workflow` folder included in the template. 
- Test your workflow to ensure it produces consistent and reproducible results. If you do not have your own test data, minimal datasets are available at [__](LINK).  
- Once complete, we suggest filling out the `LICENSE`, `README.md`, `CITATIONS.md`, `CITATION.cff`, and `CHANGELOG.md` files as specified in [_](LINK). It will help ensure that others use your pipeline appropriately and that proper credit is given to everyone who worked on the pipeline.
- Likewise, to make it easier for others to use your pipeline, we suggest [exporting your conda environment](conda_guide.md#exporting-a-conda-environment) and placing it in the `config` folder. This will make sure anyone using your pipeline has the exact same tools.

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

### From an Existing Project
#### 1. Create a new Catalogue Repository
1. In the Code Catalogue group, click the `New Project` button in the top-right corner of the page.  
2. If: 
    - your project already exists in **GitLab**, select `Import Project`:

    - your project exists **elsewhere**, select `Create blank project`:
        1. Add a ***Project name***. This will be the working name of your pipeline.
        2. Under ***Project URL***, select the `code_catalogue` namespace from the dropdown menu and add a `Project Slug`, which will be the end of the URL to your project. We recommend that it matches the name of your pipeline.
        3. Select `Private` as the visibility level. 
        4. Leave the rest as is and click `Create project`.
        

A repository should be set to `private` until it is ready to be deployed. This is to ensure that the catalogue is not filled with copies of the empty template project if a pipeline's development takes longer than expected. Individuals who have been added to the Code Catalogue group will be able to see all project repositories, even those set to private. This will only prevent the public from having to sift through empty pipelines. 
#### 2. Work on your pipeline 
We recommend creating two branches, `main` and `dev`, to keep track of pipeline changes. We suggest that all active development happens on the `dev` branch and that `main` only be used to house stable version releases of the pipeline, according to the [pipeline guidelines](pipeline_guidelines.md#suggestions). To do this:  

- Create and switch to the `dev` branch of the repository. 
    > $ git checkout dev  
- Import your pipeline files.

To make pipeline usage easier for users and analysis results more reproducable, we recommend the following:  
- [Create a conda environment](conda_guide.md#create-a-new-environment) for your project and [install](conda_guide.md#manage-conda-packages) any tools that are needed to run the pipeline. Then [export your conda environment](conda_guide.md#exporting-a-conda-environment), to make sure anyone using your pipeline has the exact same tools.
- Test your workflow to ensure it produces consistent and reproducible results. If you do not have your own test data, minimal datasets are available at [__](LINK).  
- Once complete, we suggest including `LICENSE`, `README.md`, `CITATIONS.md`, `CITATION.cff`, and `CHANGELOG.md` files as specified in [_](LINK). It will help ensure that others use your pipeline appropriately and that proper credit is given to everyone who worked on the pipeline.


## Adding your Pipeline to the Code Catalogue  
Once you're ready to add your pipeline to the code catalogue, you will need to update the `main` branch and make the repository public. To do this:  
1. Change to the `main` branch:  
    > $ git checkout main  
2. Merge the `dev` branch into `main`:  
    > $ git merge dev  
3. Go to your project page.  
4. On the left sidebar, expand `Settings` and click `General`.  
5. Expand `Visibility, project features, permissions`.  
6. Set the `Project visibility` to `Public` from the drop-down and click on `Save changes`.  

## Updating and Mainting your Pipeline  
The same method should be used when updating your pipeline. The development of new features or changes should take place in `dev` and once complete and stable, merged into `main`. Additional suggestions for pipeline updates can be found [here](pipeline_guidelines.md#pipeline-updates).  

## Contributing to Someone Else's Pipeline
 >*Do we want to do issue tickets for this as well?*
## Reporting Errors
Errors should be submitted as issue tickets. If you notice something wrong in one of the catalogue's pipelines, you can open a new issue with the following steps:  
- Click on the desired pipeline's repository page.
- On the left sidebar, click on `Issues`.
- Click on `New issue`.
- Enter a `Title` that is descriptive of the problem.
- Enter a `Description` of the problem at hand.
- Leave everything else as is and click on the `Create issue` button.