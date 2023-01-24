![](../../images/logo.png)
# NGS Metadata standard, v1.0

## Overview

The following keys are defined to described raw data from next-generation sequencing instruments.

## Defined keys

| Key | Description | Unit | Category
| --- | ----------- | ---- | --------
| BARCODE_SAMPLE | NGS Barcode of sample | String | Sequencing
| COLLECTION_DATE | Date sample was collected | Date | Sample
| COMMENT | A comment about the data | String | Generic
| COMMON_NAME | Common species name | String | Sample
| CONTACT_EMAIL | Email of primary contact | String | User
| CONTACT_NAME | Name of primary contact | String | User
| CRC_PROJECT | Name of CRC sub project | String | User
| EXPERIMENTAL_FACTOR | Experimental factor | String | Generic
| EXTERNAL_ID | External ID linking to this data | String | Generic
| EXTERNAL_ID_SOURCE | Source of external ID | String | Generic
| FLOWCELL_ID | ID of flow cell | String | Sequencing
| FLOWCELL_LANE | Lane on flow cell | Integer | Sequencing
| INVESTIGATION_TYPE | Type of investigation performed | String | Generic
| LIBRARY_CONSTRUCTION_METHOD | Method or kit used for library construction | String | Sequencing
| LIBRARY_ID | Unique identifier of a sequencing library | String | Sequencing
| LIBRARY_READ_GROUP_ID | Read group ID of library | String | Sequencing
| LIBRARY_READ_LENGTH | Length of sequence reads | String | Sequencing
| LIBRARY_READS_SEQUENCED | Number of reads sequenced | Integer | Sequencing
| LIBRARY_SAMPLE_TYPE | Sample type library was constructed from | String | Sequencing
| LIBRARY_SCREENING_STRATEGY | Strategy used to screen library | String | Sequencing
| LIBRARY_SIZE | Size of library in bp | Integer | Sequencing
| LIBRARY_VECTOR | Vector used for library construction, if any | String | Sequencing
| NUCLEIC_ACID_EXTRACTION | Protocol used to extract DNA/RNA | String | Generic
| OWNER_EMAIL | Email of data owner | String | User
| OWNER_NAME | Name of data owner | String | User
| PHENOTYPE | Pehnotype(s) as HPO terms | String | Generic
| PROJECT_NAME | Name of a project | String | Generic
| SAMPLE_ALIAS | Alias name of a sample | String | Sample
| SAMPLE_COLLECTION_DEVICE_OR_METHOD | How a sample was collected | String | Sample
| SAMPLE_DESCRIPTION | Description of a sample | String | Sample
| SAMPLE_MATERIAL_PROCESSING | Processing that was performed on sample | String | Sample
| SAMPLE_NAME | Name or identifier of sample | String | Sample
| SAMPLE_SEX | Sex of a sample/individual | String | Sample
| SAMPLE_STORAGE_DURATION | How long a sample was stored for in days | Integer | Sample
| SAMPLE_STORAGE_LOCATION | Location a sample was stored at | String | Sample
| SAMPLE_STORAGE_TEMPERATURE | Temperature the sample was stored at | °C | Sample
| SCIENTIFIC_NAME | Scientific species name | String | Sample
| SEQUENCING_CENTRE | Centre were sequencing was performed | String | Sequencing
| SEQUENCING_DATE | Date sequencing was performed | Date | Sequencing
| SEQUENCING_METHOD | Sequencing technology | String | Sequencing
| SEQUENCING_PLATFORM | Sequencing instrument | String | Sequencing
| SOURCE_MATERIAL_IDENTIFIER | Identifies a sample source material | String | Sample
| TAX_ID | NCBI Taxon ID | Integer | Sample
