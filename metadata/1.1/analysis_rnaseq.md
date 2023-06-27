![](../../images/logo.png)
# RNA-seq analysis Metadata standard, v1.1

## Overview

The following keys are defined to describe results from an RNA-seq analysis. 

## Sample sheet

Analysis Metadata sample sheet [XLSX](CRC1526_RNAseq_Analysis.xlsx)

## Defined keys

| Key | Description | Unit | Category
| --- | ----------- | ---- | --------
| comment | A comment about the data | String | Generic
| contact_email | Email of primary contact | String | User
| contact_name | Name of primary contact | String | User
| crc_project | Name of CRC sub project | String | User
| external_id | An external ID linking to this data from another source, like an in-house database or public repository. To be used in combination with external_id_source. | String | Generic
| external_id_source | Specifies the source an external id points to. This can be an in-house repository or a public database. | String | Generic
| file_format | Format used to store data | String | Generic
| owner_email | Email of data owner | String | User
| owner_name | Name of data owner | String | User
| pipeline | Name of pipeline used | String | Analysis
| pipeline_github_url | Github URL of pipeline project used | String | Analysis
| pipeline_options | Options passed to pipeline | String | Analysis
| pipeline_version | Version or commit hash of pipeline | String | Analysis
| project_name | Name of a project | String | Generic
| sample_list | A comma-separated list of unique identifiers that were used in this analysis | String | Analysis
| sample_list_source | The source where the sample_list identifiers come from | String | Analysis
