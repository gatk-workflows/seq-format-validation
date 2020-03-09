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
 - Successfully tested on v49
 - Does not work on versions < v23 due to output syntax

### Important Notes :
- Runtime parameters are optimized for Broad's Google Cloud Platform implementation.
- The provided JSON is a ready to use example JSON template of the workflow. Users are responsible for reviewing the [GATK Tool and Tutorial Documentations](https://gatk.broadinstitute.org/hc/en-us/categories/360002310591) to properly set the reference and resource variables. 
- For help running workflows on the Google Cloud Platform or locally please
view the following tutorial [(How to) Execute Workflows from the gatk-workflows Git Organization](https://gatk.broadinstitute.org/hc/en-us/articles/360035530952).
- Relevant reference and resources bundles can be accessed in [Resource Bundle](https://gatk.broadinstitute.org/hc/en-us/articles/360036212652).

### Contact Us :
- The following material is provided by the Data Science Platforum group at the Broad Institute. Please direct any questions or concerns to one of our forum sites : [GATK](https://gatk.broadinstitute.org/hc/en-us/community/topics) or [Terra](https://support.terra.bio/hc/en-us/community/topics/360000500432).

### LICENSING :
Copyright Broad Institute, 2019 | BSD-3
This script is released under the WDL open source code license (BSD-3) (full license text at https://github.com/openwdl/wdl/blob/master/LICENSE). Note however that the programs it calls may be subject to different licenses. Users are responsible for checking that they are authorized to run all programs before running this script.
