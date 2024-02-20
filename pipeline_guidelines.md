# Guidelines  

## Introduction  

## Requirements  
All AAFC pipelines ***must*** follow the following guidelines:  
- (DO WE WANT TO ENFORCE A SPECIFIC WORKFLOW MANAGER? For example, nf-core pipelines MUST use nextflow)  
- **Pipeline Specificity**: There should only be a single pipeline for each type of data or analysis. Redundant pipelines should not be created and will not be included in this catalogue.  
- **Pipeline name**: Names should be descriptive of the overall function of the pipeline. Names should be lowercase, without punctuation. If multiple words are needed, seperate them with an '_'.  
- **Use the template**: All AAFC pipelines must be built using the provided [AAFC pipeline template](LINK).  
- **License**: Each pipeline must include a usage license on release. The code catalogue provides a version of the [MIT license](LINK) if needed.
- **Documentation**: All necessary documentation must be included with the pipeline and hosted in the AAFC catalogue.
- **Conda support**: Software must be packaged using [Conda](LINK) and an environment file must be included. For more info refer to the [Conda Guide](conda_guide.md).  
- **Credits and Acknowledgements**: Pipelines must properly cite used software and acknowledge work done by others. A  [template](CITATIONS.md) has been provided.
- **Citation**: Information on how to cite the pipeline should be included. A [CITATION.cff file template](CITATION.CFF) has been included and should be filled out according to the [following examples](https://docs.github.com/fr/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files#about-citation-files).  

## Pipeline Updates  
Each contributor is responsible for the publication and maintenance of their own pipeline.  

Updates must follow the following guidelines:  
- **Semantic versioning**: Pipelines must use stable release tags.
- **Use git branches**: Use `main` and `dev` branches to differentiate stable and in-progress versions of the pipeline. 
- **Changelog**: All changes should be documented in [CHANGELOG.md](CHANGELOG.md). 

## Submission Process  
If you would like your pipeline to be listed in the AAFC code catalogue, please submit it through [__](LINK).  

Once submitted, a member of the core team will review the submission for compliance with the above guidelines. If your submission fullfils all the pipeline requirements, it will be added to the catalogue and marked as `complete`. If your submission is missing certain required sections, it will be added but marked as `in progress`, and the missing sections will be indicated in the pipeline's tags. 

When updates are submitted, a core team member will likewise review those updates for compliance with AAFC code catalogue guidelines.

## Violations  

If a pipeline is found to be violating the AAFC guidelines after being added to the code catalogue, the following actions will be taken in order to correct the situation:  
1. A member of the core team will assess what changes need to be made and contact the person responsible for the pipeline about their recommendations. 
2. Based on the assessment, the pipeline may be tagged as `in progress` until it conforms to the code catalogue guidelines, or may be archived or removed from the catalogue.   

All members of the AAFC community must adhere to the code catalogue's [code of conduct](LINK). Adherence to the code of conduct takes precedence over the development guidelines described in this page.


//everyone is responsible for their own publication. code catalogue responsable will review?
If in doubt on any of the points above, please [ask a core team member](LINK) for clarification. 