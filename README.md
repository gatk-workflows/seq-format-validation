# seq-validation
Workflows for validating sequence data
### validate-bam :
 This WDL performs format validation on SAM/BAM files in a list

#### Requirements/expectations :
 - One or more SAM or BAM files to validate
 - Explicit request of either SUMMARY or VERBOSE mode in inputs.json

#### Outputs:
 - Set of .txt files containing the validation reports, one per input file

### Cromwell version support 
 - Successfully tested on v312
 - Does not work on versions < v23 due to output syntax

 Runtime parameters are optimized for Broad's Google Cloud Platform implementation. 
 For program versions, see docker containers. 
