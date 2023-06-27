![](../../images/logo.png)
# NGS Metadata standard, v1.1

## Overview

The following keys are defined to described raw data from next-generation sequencing instruments.

## Sample sheet

NGS Metadata sample sheet [XLSX](CRC1526_NGS_data_v1.xlsx)

## Defined keys

| Key | Description | Unit | Category
| --- | ----------- | ---- | --------
| adapters | Adapters provide priming sequences for both amplification and sequencing of the sample-library fragments | String | Sequencing
| collection date | The date the sample was collected with the intention of sequencing, either as an instance (single point in time) or interval | String | Undefined
| comment | A comment about the data | String | Generic
| common name | Common species name | String | Sample
| contact email | Email of primary contact | String | User
| contact name | Name of primary contact | String | User
| crc project | Name of CRC sub project | String | User
| experimental factor | Experimental factors are essentially the variable aspects of an experiment design which can be used to describe an experiment, or set of experiments, in an increasingly detailed manner | String | Generic
| external id | An external ID linking to this data from another source, like an in-house database or public repository. To be used in combination with external_id_source. | String | Generic
| external id source | Specifies the source an external id points to. This can be an in-house repository or a public database. | String | Generic
| flowcell id | ID of flow cell | String | Sequencing
| investigation type | Nucleic Acid Sequence Report is the root element of all MIxS compliant reports as standardised by Genomic Standards Consortium | String | Generic
| library construction method | Library construction method used for clone libraries | String | Sequencing
| library id | Unique identifier of a sequencing library. Usually, this will be part of the name of a sequence file. | String | Sequencing
| library read group id | The unique read group ID of a set of reads. | String | Sequencing
| library read length | Length of sequence reads | String | Sequencing
| library reads sequenced | Total number of clones sequenced from the library | String | Sequencing
| library sample type | Sample type library was constructed from | String | Sequencing
| library screening strategy | Specific enrichment or screening methods applied before and/or after creating clone libraries in order to select a specific group of sequences | String | Sequencing
| library size | Total number of clones in the library prepared for the project | String | Sequencing
| library vector | Cloning vector type(s) used in construction of libraries | String | Sequencing
| miscellaneous parameter | Any other measurement performed or parameter collected, that is not listed here | String | Generic
| nucleic acid amplification | A link to a literature reference, electronic resource or a standard operating procedure (SOP), that describes the enzymatic amplification (PCR, TMA, NASBA) of specific nucleic acids | String | Sequencing
| nucleic acid extraction | A link to a literature reference, electronic resource or a standard operating procedure (SOP), that describes the material separation to recover the nucleic acid fraction from a sample | String | Sequencing
| owner email | Email of data owner | String | User
| owner name | Name of data owner | String | User
| phenotype | Where possible, please use the Experimental Factor Ontology (EFO) to describe your phenotypes. | String | Generic
| project name | Name of the project within which the sequencing was organized | String | Generic
| relevant standard operating procedures | Standard operating procedures used in assembly and/or annotation of genomes, metagenomes or environmental sequences in the format of a PMID, DOI or URL | String | Generic
| sample alias | Alias name of a sample | String | Sample
| sample barcode | NGS Barcode of sample | String | Sequencing
| sample collecting device or method | How a sample was collected | String | Sample
| sample description | Description of a sample | String | Sample
| sample material processing | A brief description of any processing applied to the sample during or after retrieving the sample from environment, or a link to the relevant protocol(s) performed. | String | Sample
| sample name | Unique name or identifier of a biological sample. | String | Sample
| sample sex | Sex of a sample/individual | String | Sample
| sample storage duration | duration for which sample was stored | days,hours,months,weeks,years | Sample
| sample storage location | location at which sample was stored, usually name of a specific freezer/room | String | Sample
| sample storage temperature | temperature at which sample was stored, e.g. -80 | °C | Sample
| sample volume or weight for dna extraction | Total sample volume (ml) or weight (g) processed for DNA extraction | String | Sample
| scientific name | Scientific species name | String | Sample
| sequencing centre | Centre were sequencing was performed | String | Sequencing
| sequencing date | Date sequencing was performed | Date | Sequencing
| sequencing method | Sequencing machine used | String | Sequencing
| sequencing platform | Sequencing instrument | String | Sequencing
| source material identifier | Identifies a sample source material | String | Sample
| tax id | NCBI Taxon ID, such as 9606 for human or 10090 for mouse. | Integer | Sample
