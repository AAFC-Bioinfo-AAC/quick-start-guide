# AAFC Pipeline Creation Guide
[[_TOC_]] 



## Creating a Pipeline
### Before Starting
The AAFC Code Catalogue is __ . Before creating a pipeline, make sure that you take a look at the pipelines that have already been created or are in development and are familiar with the pipeline [requirements](pipeline_guidelines.md) and [git basics](LINK).  

Once you have an idea for a workflow you'd like to contribute to the Code Catalogue, submit a [pipeline proposal form](LINK) to confirm that it does not overlap with other pipelines that are in development or that have been suggested. This form will be reviewed by a member of the Code Catalogue team, who will confirm the uniqueness of your proposed pipeline. If it is too similar, consider contributing to the already existing pipeline or collaborating with others who have suggested a similar project. A core team member will be able to put you in contact with the persons in question.  

### Create the pipeline
>*Assuming we have a template repo.*  

>*Implementation differs depending on if we are using github or gitlab in the end, so I will not fill out the details of this section just yet.* 
>- *If Github, fork the template repository to new local repository. Steps will be inserted.* 
>- *If Gitlab, select create new repository from template, and then select group templates and select the code catalogue pipeline template. Create the new repository locally. Steps will be inserted.*

>*If we cannot have a template repo, then we have a few options.*
 >- *The user can manually download the template files and arrange them into the proper configuration within their own local repo. Pros: no additional strain on our resources. Cons: they could improperly set up their repo, and it is more tedious for the user.*
 >- *We could likewise follow the nf-core method. When a pipeline is approved, we will need to create a repo for the user.Pros: Consistent repos. Easy for user. Cons: it will be more work for the person/persons in charge of the catalogue.*

 >*Additional option of housing the template repo on github and then housing the catalogue in gitlab, since pipelines will need to be manually reviewed to be added to the catalogue anyways. We could instruct the user to create a local repo by forking the github template. We then review their repo before importing it to the gitlab catalogue.*

A repository is only added to the Code Catalogue once it is ready to be deployed. This is to ensure that the catalogue is not filled with copies of the template project when a pipeline's development takes longer than expected. To begin then, you'll need to create a local project repository by __.  

## Adding your Pipeline to the Code Catalogue

## Updating your Pipeline