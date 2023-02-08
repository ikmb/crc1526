![](../../images/logo.png)
# NGS Metadata standard, v1.0

## Overview

The following keys are defined to described raw data from next-generation sequencing instruments.

## Sample sheet

NGS Metadata sample sheet [XLSX](CRC1526_NGS_data_v1.xlsx)

## Defined keys

| Key | Description | Unit | Category
| --- | ----------- | ---- | --------
| collection_date | Date sample was collected | Date | Sample
| comment | A comment about the data | String | Generic
| common_name | Common species name | String | Sample
| contact_email | Email of primary contact | String | User
| contact_name | Name of primary contact | String | User
| crc_project | Name of CRC sub project | String | User
| experimental_factor | A specific experimental factor that was applied to this sample (e.g. low-calory diet) | String | Generic
| external_id | An external ID linking to this data from another source, like an in-house database or public repository. To be used in combination with external_id_source. | String | Generic
| external_id_source | Specifies the source an external id points to. This can be an in-house repository or a public database. | String | Generic
| flowcell_id | ID of flow cell | String | Sequencing
| flowcell_lane | Lane on flow cell | Integer | Sequencing
| investigation_type | Type of investigation performed | String | Generic
| library_construction_method | Method or kit used for library construction | String | Sequencing
| library_id | Unique identifier of a sequencing library. Usually, this will be part of the name of a sequence file. | String | Sequencing
| library_read_group_id | The unique read group ID of a set of reads. | String | Sequencing
| library_read_length | Length of sequence reads | String | Sequencing
| library_reads_sequenced | Number of reads sequenced | Integer | Sequencing
| library_sample_type | Sample type library was constructed from | String | Sequencing
| library_screening_strategy | Strategy used to screen library | String | Sequencing
| library_size | Size of library in bp | Integer | Sequencing
| library_vector | Vector used for library construction, if any | String | Sequencing
| miscellaneous_parameter | further descriptions, if needed | String | Generic
| nucleic_acid_amplification | Amplification protocol used, if any | String | Sequencing
| nucleic_acid_extraction | Protocol used to extract DNA/RNA | String | Sequencing
| owner_email | Email of data owner | String | User
| owner_name | Name of data owner | String | User
| phenotype | Phenotype(s) as HPO terms | String | Generic
| project_name | Name of a project | String | Generic
| relevant_standard_operating_procedures | Standard operating procedures used for data production | String | Generic
| sample_alias | Alias name of a sample | String | Sample
| sample_barcode | NGS Barcode of sample | String | Sequencing
| sample_collecting_device_or_method | How a sample was collected | String | Sample
| sample_description | Description of a sample | String | Sample
| sample_material_processing | Processing that was performed on sample | String | Sample
| sample_name | Unique name or identifier of a biological sample. | String | Sample
| sample_sex | Sex of a sample/individual | String | Sample
| sample_storage_duration | How long a sample was stored for in days | Integer | Sample
| sample_storage_location | Location a sample was stored at | String | Sample
| sample_storage_temperature | Temperature the sample was stored at | °C | Sample
| sample_volume_or_weight_for_dna_extraction | Total sample volume (ml) or weight (g) processed for DNA extraction | String | Sample
| scientific_name | Scientific species name | String | Sample
| sequencing_centre | Centre were sequencing was performed | String | Sequencing
| sequencing_date | Date sequencing was performed | Date | Sequencing
| sequencing_method | Name of the sequencing technology (e.g. Illumina short-read sequencing) | String | Sequencing
| sequencing_platform | Sequencing instrument | String | Sequencing
| source_material_identifier | Identifies a sample source material | String | Sample
| tax_id | NCBI Taxon ID, such as 9606 for human or 10090 for mouse. | Integer | Sample
