# Guidelines  

## Introduction  

## Requirements  
All AAFC pipelines ***must*** follow the following guidelines:  
- (DO WE WANT TO ENFORCE A SPECIFIC WORKFLOW MANAGER? Example, nf-core pipelines MUST use nextflow)  
- **Pipeline Specificity**: There should only be a single pipeline for each type of data or analysis. Redundant pipelines should not be created and will not be included in this catalogue.  
- **Pipeline name**: Names should be descriptive of the overall pipeline use. Names should be lowercase, without punctuation. If multiple words are needed, seperate them with an '_'.  
- **Use the template**: All AAFC pipelines must be built using the provided [AAFC pipeline template](LINK).  
- **License**: Each pipeline must include AAFC's version of the MIT license on release (included in the template).
- **Documentation**: All necessary documentation must be included with the pipeline and hosted in the AAFC catalogue.
- **Conda support**: Software must be packaged using [Conda](LINK) and an environment file must be included.  
- **Credits and Acknowledgements**: Pipelines must properly cite used software and acknowledge work done by others.
- **Citation**: Information on how to cite the pipeline should be included. (Do we want to make DOIs mandatory?)  

## Violations
