# Guidelines  

## Introduction  

## Suggestions  
All Code Catalogue pipelines ***should*** follow the following guidelines:  
- **Workflow Management**: We suggest using either [Nextflow](https://www.nextflow.io/) or [Snakemake](https://snakemake.github.io/) for pipelines with many steps. This will avoid having to run the entire pipeline when small updates are made to the pipeline or input data.
- **Pipeline Specificity**: There should only be a single pipeline for each type of data or analysis. Redundant pipelines should not be created or included in this catalogue to minimize clutter and wasted time.
- **Pipeline name**: Names should be descriptive of the overall function of the pipeline to make searching for relevant pipelines easier. Names should be lowercase, without punctuation, and use underscores to seperate words.   
- **Use the template**: All AAFC pipelines should be built using the provided [AAFC pipeline template](LINK).  
- **License**: Each pipeline should include a usage license on release. The code catalogue provides a version of the [MIT license](LINK) if needed.
- **Documentation**: All necessary documentation should be included with the pipeline and hosted in the AAFC catalogue so that users know how to properly use the pipeline.
- **Conda support**: Software should be packaged using [Conda](LINK) and an environment file should be included in the pipeline. For more info refer to the [Conda Guide](conda_guide.md).  
- **Credits and Acknowledgements**: Pipelines should properly cite used software and acknowledge work done by others. A [template](CITATIONS.md) has been provided.
- **Citation**: Information on how to cite the pipeline should be included so that you are properly credited for your work. A [CITATION.cff file template](CITATION.CFF) has been included and can be filled out according to the [following examples](https://docs.github.com/fr/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files#about-citation-files).  

## Pipeline Updates  
Each contributor is responsible for the publication and maintenance of their own pipeline.  

Updates should follow the following guidelines:  
- **Semantic versioning**: Pipelines should use stable release tags.
- **Use git branches**: Use `main` and `dev` branches to differentiate stable and in-progress versions of the pipeline. 



## Code of Conduct  

All members of the Code Catalogue community must adhere to the code catalogue's [code of conduct](LINK).  
If a pipeline is found to be in violation of the [code of conduct](LINK), the following actions will be taken in order to correct the situation:    
1. A member of the core team will set the repository to `private`, asses what changes need to be made and contact the person responsible for the pipeline about their recommendations. 
2. If it is not changed to conform to the code of conduct, the pipeline may be removed from the catalogue.   
  
## Questions? 
If in doubt on any of the points above, please [ask a core team member](LINK) for clarification, we'd be happey to help. 