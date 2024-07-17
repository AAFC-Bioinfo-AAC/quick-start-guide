# Guidelines for code and pipelines
## For code   

In order to make the code catalogue repositories follow FAIR principles: Findable, Accessible, Interoperable and Reusable, consider adhering to the following guidelines.**TBD**   

 >Add code linting, comments, etc.

## For pipelines   

All Code Catalogue pipelines ***should*** follow the following guidelines as far as possible:   

 

- **Workflow Management**: Use [Nextflow](https://www.nextflow.io/) or [Snakemake](https://snakemake.github.io/) where possible. 

 

- **Pipeline Specificity**: There should only be a single pipeline for each type of analysis, unless there is a case for an alternative implementation. If an existing pipeline doesn’t exactly meet your needs, consider collaborating with the creator to add necessary functionality or creating a branch of the pipeline with your changes. 

 

- **Pipeline name**: Names should be descriptive of the overall function of the pipeline to make repositories **findable**. If [Nextflow](https://www.nextflow.io/) or [Snakemake](https://snakemake.github.io/) are used in your pipeline, add `NF` (for nextflow) or `SM` (for snakemake) to the end of the name. Names should be lowercase, without punctuation, and use underscores to separate words. Tags may be added to categorize the pipeline to broad/pre-defined categories.   

 

- **Use the pipeline template**: All AAFC pipelines should be built using or added to the provided [AAFC pipeline template](https://gccode.ssc-spc.gc.ca/abcc_rcba/abcc_rcba_pipeline_template).   

 

- **License**: Each pipeline should include a usage license on release. Information on choosing the right license can be found [here](https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/open-source-software/guide-for-publishing-open-source-code.html#toc04). It is your responsibility to ensure the repositories you maintain include the correct license for your use-case. 

 

- **Documentation**: Repositories should include the necessary documentation to install and use the pipeline. It is also advisable to include a minimal test input dataset and a description of the expected output(s). 

 

- **Conda support**: Software should be packaged using [Conda](https://conda.io/projects/conda/en/latest/index.html) and an environment file should be included in the pipeline. For more info refer to the [Conda Guide](https://github.com/GRDI-GenARCC/tutorials-and-workshops/tree/main/Conda).   

 

- **Credits and Acknowledgements**: Pipelines should properly cite used software and acknowledge work done by others. A [template](https://gccode.ssc-spc.gc.ca/abcc_rcba/abcc_rcba_pipeline_template/-/blob/main/CITATIONS.md?ref_type=heads) has been provided. 

 

- **Citation**: Information on how to cite the pipeline should be included so that you are properly credited for your work. A [CITATION.cff file template](https://gccode.ssc-spc.gc.ca/abcc_rcba/abcc_rcba_pipeline_template/-/blob/main/CITATION.cff?ref_type=heads) has been included and can be filled out according to the [following examples](https://docs.github.com/fr/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files#about-citation-files).   

 

## Pipeline Updates   

Each contributor is responsible for the publication and maintenance of their own pipeline.   

Updates should follow these guidelines:   

- **Semantic versioning**: Pipelines should use [stable release tags](https://semver.org/). 

- **Use git branches**: Use `main` and `dev` branches to differentiate stable and in-progress versions of the pipeline.  

 

## Code of Conduct   

All members of the Code Catalogue community must adhere to the code catalogue's [code of conduct](CODE_OF_CONDUCT.md).   

If a pipeline is found to be in violation of the code of conduct, the following actions may be taken in order to correct the situation:     

1. The offending repository will be set to `private`. The repository maintainer will be contacted and informed of the necessary changes. Once the repository is updated to adhere to the code of conduct, it will be restored to public status. 

2. Failure to correct the repository to adhere to the code of conduct in a timely fashion may result in the removal from the code catalogue.    


## Questions?  

If in doubt on any of the points above, please [ask a core team member](README.md#how-to-contact) for clarification, we'd be happy to help.  