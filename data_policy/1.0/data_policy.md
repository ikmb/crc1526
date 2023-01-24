# Data policy, version 1.0

## Overview 
 
This document outlines the data management and release policy for the collaborative research centre (CRC) “CRC1526”. The goal of this document is to provide instructions on how data is to be stored, described, accessed and disseminated.  
 
Within this document, the term “data” is primarily used to refer to sequencing data (both genome and RNA level) generated as part of research projects within the CRC. This data may come from model organisms or patients (see #Clinical-Data). Additional data types may be adequately covered by the general instructions below. If existing rules seem unsuitable for a given type of data, amendments to this document under Section 3 shall be made in dialogue with the INF project.   
 
## Roles and responsibilities 
 
The following roles and associated responsibilities are currently defined: 

### Medical HPC research cluster, Lübeck University 
 
The administrative team overseeing the operation of the medical computing cluster “Omics Cluster” at Lübeck University provides the IT infrastructure required for the CRC data management. This data management system is referred to as “Pantau-Omics”.  
 
The administrative team ensures that services are maintained and expanded as required by the CRC1526.   
 
### CRC1526 INF project 
 
The INF project is responsible for implementing data life cycles and workflows. Most of the “primary” data will be handled by the INF project and processed according to the guidelines outlined in the present data policy (Section 3 and 4). 
 
### Data producers / PIs 
 
Principal investigators within the CRC are responsible for communicating their data generation plans to the INF project to ensure that all data can be captured in the data management system of the CRC.  
 
The INF project, where possible, shall be designated a data recipient for all sequencing projects. 
 
PIs must ensure that metadata is captured prior to e.g. sequencing and passed on to the INF project. The INF project can provide appropriate forms for standard applications.  

The choice of metadata to include lies (primarily) with the data producers but shall be in accordance with “FAIR” principles (i.e. third parties must be able to reuse the data given the annotated metadata). 

### All users 
 
All users of the data management system must comply with data access and release policies outlined in Section 4. 
 
## Storage and annotation 
 
### iRODS archive storage 
 
All raw (sequencing) data (both genome and RNA) generated within the CRC (i.e. financed through CRC funds) must be deposited in the data management solution “Pantau-Omics”.  
 
If sequencing is not coordinated with the INF project for automatic data delivery/archiving, it is the users’ responsibility to ensure that data is deposited with all relevant metadata (Section 3.2). 
 
Analytical results based on these raw data may be submitted to the data management system, together with a description on how this information was generated. For further details regarding data types, see Section 3.    
 
Data not generated as part of the CRCs’ activities must not be deposited  in the “Pantau-Omics” system, unless specifically authorised by the INF project.  
 
Individual data sets consisting of multiple files should be combined into one “tar” archive and uploaded as a single object. A thusly created tar archive shall represent a given state within the research project (e.g. raw data or analytical results). Different data stages may not be mixed into one tar object (e.g. data and results) but should reference each other via metadata keys.  
 
Data shall be deposited in the iRODS folder of the corresponding research project the data was generated for.  
 
Data access shall be set in accordance with guidelines described under Section 4.  
 
Data will be stored within the “Pantau-Omics” system for the lifetime of the CRC, but at minimum 3 years from initial submission into the system.  
 
Storage beyond this time should be sought through publication to international data repositories (Section 4.2).   
 
### Metadata annotation 
 
All data submitted to the data management system must be annotated with relevant metadata to enable data discovery across projects within the CRC, help with submission to downstream repositories and enable third parties to reuse the data at a later point. The current metadata standard for the CRC is described under: 
 
https://github.com/ikmb/crc1526
 
These specifications are based on the EBI MIxS standard (http://www.ebi.ac.uk/ena/submit/mixs-checklists). Metadata keys not covered by this specification should be used only after consulting with the INF project so they can be added to the metadata vocabulary.  

### Clinical data

Clinical (patient) data will be managed by the Z1 project and is not covered by this data policy. All digital data subject to this data policy shall be anonymised and must not include metadata directly enabling identification of individuals or allow linking FROM the raw data to patient data. Specifically, no identifying information, such as a patient ID or name, shall be stored.  Connecting clinical data with digital/omics data shall only be possible through the Z1 project - using information about the relationship of probant identities (Z1) and e.g., sequencing library identifiers (INF) or internally agreed-upon pseudonyms.  

## Data types 
 
### Short read files (fastq or ORA) 
 
Short reads generated on e.g. the Illumina platform of machines are the primary data type within the CRC.  
 
Short reads shall be deposited within the  “Pantau-Omics” in their raw form (no trimming, no filtering), with their original file name as given by the sequencing provider intact.  
 
For efficient usage of the storage system, read files shall be compressed using one of two algorithms. If possible, the Illumina ORA format shall be used. Instructions for this will be provided separately by the INF project. If ORA compression is not possible, the GZIP algorithm shall be used - following the naming convention “.fastq.gz”. 

Compressed raw data must be accompanied by an md5sum to allow data integrity checks.  
 
Where multiple read files belong to one sample (i.e. paired-end reads), the compressed files shall be grouped into one tar archive. The tar archive shall be named after the sequencing library (usually the common root of the filenames to be grouped).  
 
The tar archive shall contain the corresponding fastqc statistics (one statistics file per sequence file).  
 
### Genotyping data

Genotyping data are the second primary data type generated within CRC1526. Genotyping data shall be stored in PLINK format (bim/bed/fam) and must include the data-producer supplied manifest file (CSV). Metadata for genotyping data must include information on the chip and reference assembly against which calling was performed. 

### Analytical results (generic) 
 
Finalised analyses (tabular counts or similar) may only be stored in “Pantau-Omics” if the analysis process is included with the data so that any user may be able to accurately reproduce the workflow. Analysis and the “analysis trace” shall be submitted together as tar archive and must be annotated with appropriate metadata. Specifically, it must be clear which raw data was used in the analysis by reference to the sample or library name(s) within "Pantau-Omics".  
 
The format of the analytical result must be discussed with the INF project prior to submission to help identify common standards and develop best practices.  
 
## Access and release 
 
### Data sharing within the CRC 
 
Data and metadata from the individual projects shall be readable by all CRC members to aid in data discovery.  
 
Data shall only be writable by members of the respective projects (the data owner).  
 
Data belongs to the user it was generated for, as indicated by the mandatory metadata key “MAIN_CONTACT_NAME”.  
 
Any use of the data prior to its publication needs permission by the owner.   
 
### Release of data into the public domain 
 
Data generated within the CRC shall be made available to the public upon publication.  
 
Data shall be published through upload into suitable, widely accepted repositories (e.g. NCBI or EBI archives).  
 
Data published to international repositories shall be annotated within the CRC iRODS using the resulting digital object identifier (DOI) in the remote database, if possible/applicable.  
 
### Revision history 
 
Draft 1 generated in January 2023. 
 
Release 0.1 generated in 01/2023

