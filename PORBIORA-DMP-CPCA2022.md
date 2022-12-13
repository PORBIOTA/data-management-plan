# DMP – PORBIOTA-Portuguese e-Infrastructure for Information and Research on Biodiversity

## Scope of this DMP

This DMP was prepared in the scope of the call FCT-CPCA-2022 (proposal 2022.15827.CPCA)
and includes the relevant parts of the full DMP of PORBIOTA related to the use of
scientific cloud computing services for INCD STRATUS by PORBIOTA.

It includes the following components of PORBIOTA:
- biodiversity data publication and use through GBIF
- image long term archiving of collection specimens
- long term archiving of spectral data and associated vegetation
photographs
- carbon and water fluxes

The DMP follows the template proposed by FCT for the call.

## Date and version

This DMP was created in 13-12-2022.

The last update was 13-12-2022.

The current version is Version 1.0.

The version history of the document is the following:

| Version | Date       | Authors     | Change description |
|---------|------------|-------------|--------------------|
| 1.0     | 13-12-2022 | Rui Figueira | creation of the DMP |

## Document repository

This document is deposited and updated through [https://github.com/PORBIOTA/data-management-plan/blob/main/PORBIORA-DMP-CPCA2022.md](https://github.com/PORBIOTA/data-management-plan/blob/main/PORBIORA-DMP-CPCA2022.md).
 
## 1. What data will be collected or produced, and what existing data will be re-used?

### 1.1. Which existing data you will re-use and under which terms of use.

The types of data covered in this DMP are:
1. biodiversity species occurrence data published through GBIF
2. images of herbarium collection specimens digitized
3. spectral vegetation data and images (photographs)
4. carbon fluxes

*1. Biodiversity species occurrence data published through GBIF* 

**Data Publisher Agreement terms** 

These data are published by institutions registered as publishers in GBIF. 
The [GBIF Data Publisher Agreement](https://www.gbif.org/terms/data-publisher) is 
agreed by all institutions at the time of registry. The [Portuguese Node of 
GBIF](https://www.gbif.pt), which is a member of PORBIOTA, engages with publisher 
institutions to ensure the full understanding of the Terms.

**Data license**

All datasets published through GBIF must adopt one of the following standard Creative
Commons licenses: Creative Commons Zero (CC0 1.0), Creative Commons Attribution 
(CC-BY 4.0) or Creative Commons Attribution Non-Commercial (CC-BY-NC 4.0). These 
define the term of use, which are human and machine-readable. The GBIF Portuguese
Node works with data publisher to recommend the use of the first two licenses, 
which are open data.

The sources of data may include the following:
- preserved specimen data from biological and natural history collections
- human observations of species occurrences
- machine observations of species occurrences (e.g. camera traps)
- literature
- remote sensing
- DNA samples

The type of publisher institutions include the following:
- Museums
- Governmental agencies and ministries
- Field science and projects
- Citizen science
- Private companies
- Universities and research units

**Data format**

Data are published through GBIF using the [Darwin Core standard](https://www.tdwg.org/standards/dwc/), 
which is managed by [Biodiversity Information Standards (TDWG)](https://www.tdwg.org/). 

**Data volume**

The current total volume of data published through GBIF, using the Integrated 
Publishing Toolkit (IPT) managed by the Portuguese GBIF Node is 10 GB.

**Data access**
Data is available for research and public use through GBIF (https://www.gbif.org/country/PT/publishing) 
and through the Biodiversity Data Portal of Portugal
(https://metadados.gbif.pt/).


*2. Images of herbarium collection specimens digitized*

PORBIOTA is promoting the digitization of specimens from herbarium collections. 
Each herbarium sheet digitized in high-resolution (400 dpi) generates a 120 MB tiff
file. As an example, view the [digitization workflow](https://dissco.github.io/HerbariumSheets/LISIULisboa.html) 
implemented by Instituto Superior de Agronomia, Universidade de Lisboa, 
in the scope of PORBIOTA.

Images are made available for use as associated media to the data publication 
through GBIF, using the Darwin Core term [associatedMedia](https://dwc.tdwg.org/terms/#dwc:associatedMedia), 
or a [Darwin Core extension](https://rs.gbif.org/extension/gbif/1.0/multimedia.xml). 

In this case, the image license is defined by the publisher, normally also using 
one of the Creative Commons licenses CC0, CC-BY or CC-BY-NC.

The archiving of images in INCD STRATUS cloud includes images files in a 
non-destructive format (normally tiff) and image metadata using relevant Darwin 
Core standard or Darwin Core Extension terms.

The current storage requirements are 7 TB.

*3. Spectral vegetation data and images (photographs)*

Contains spectral readings of vegetation from Mediterranean woodlands, for long
term preservation. It includes photograph images of the plants sampled. This 
archive is not used for data access. Data is published through Zenodo ([https://doi.org/10.5281/zenodo.5176824](https://doi.org/10.5281/zenodo.5176824)). The data license used is CC-BY-NC 4.0.

The current storage requirements are 3 GB.


*4. Carbon fluxes*

This component is not implemented yet. It will ensure future long term preservation 
of data related to the component ICOS of PORBIOTA. Data is produced by observations 
of detailed measurements of meteorological variables, the soil and the 
concentration of greenhouse gases with high temporal resolution (30') carried 
out in experimental areas in the field.

Data format follows the recommendations of the related ESFRI RI [ICOS ERIC](https://www.icos-cp.eu/), 
to which this component of PORBIOTA expects to join in the future. 

At the same time, in the same areas, we are also collecting spectral observations 
of vegetation and other essential measurements to understand the variability of 
carbon sequestration in terrestrial ecosystems.

A sample dataset of this component was already published via ZENODO 
(https://doi.org/10.5281/zenodo.3727798), using the license CC-BY 4.0.


### 1.2. If new data will be produced: describe the data you expect your research will generate and the format and volumes to be collected or produced.

All types of data described in the previous item are expected to be continuously
produced in the continuation of PORBIOTA and member institution activities. The 
expected format and storage required are described in the table bellow.

| Component | Data format | Yearly storage increment (GB) | Total data volume (GB) |
|-----------|-------------|------------------------|-------------------|
| 1. Species occurrences | Darwin Core standard (csv files) |  2.5 | 15 |
| 2. Specimen images | image (tiff, jpeg) | 1200 | 9000 |
| 3. Spectral data | csv, jpeg |  1 | 4 |
| 4. Carbon fluxes | csv, jpeg | 2500 | 5000 |

### 1.3. How much data storage will your project require in total?

More than 1000 GB.

## 2. What metadata and documentation will accompany the data?

### 2.1. Indicate what documentation will accompany the data.

1. Species occurrences data

Datasets published though GBIF include metadata following the GBIF Metadata Profile 
Version 2.1, which is a specific profile for GBIF, which uses a subset of the 
[Ecological Metadata Language (EML)](https://sbclter.msi.ucsb.edu/external/InformationManagement/EML_211_schema/docs/eml-2.1.1/index.html) standard. EML is 
used by other biodiversity-related infrastructures like eLTER-RI.

Metadata is added to each dataset in the platform [Integrated Publishing Toolkit (IPT)](https://www.gbif.org/ipt), an open source platform developed by GBIFto enable data
publication.

The following element are included in metadata profile used:
- Dataset (Resource)
- Project
- People and Organizations
- Keyword Set (General Keywords)
- Coverage
    - Taxonomic Coverage
    - Geographic Coverage
    - Temporal Coverage
- Methods
- Intellectual Property Rights
- Additional Metadata + NCD (Natural Collections Descriptions Data) Related

2. Specimen images
Specimen images are published as associated media to the specimen data published 
through GBIF. Therefore, they are covered by the metadata included in tha publication,
detailed above.

3. Spectral data
Spectral data publication in the scope of PORBIOTA is still in first stages. The 
publication. The published dataset ([https://doi.org/10.5281/zenodo.5176824](https://doi.org/10.5281/zenodo.5176824)) included
the following metadata descriptors:
- Site description
- Reflectance measurements
- File description
- Project funding
- data file structure description

4. Carbon fluxes
Carbon fluxes data publication is also in the initial phases. Metadata descriptors
of the published dataset (https://doi.org/10.5281/zenodo.3727798) includes a [metadata
file](https://zenodo.org/record/3727798/files/metadata.pdf?download=1) also based in EML that includes:
- Dataset (Resource)
- People and Organizations
- Keyword Set (General Keywords)
- Site description
- Measurements
- Data processing


### 2.2. Indicate which metadata will be provided to help others identify and discover the data.

All datasets have a DOI allocated at the publication time, either allocated by GBIF
or by Zenodo (for datasets of type 3 and 4). The metadata in each publication platform
became indexed by Google and similar indexation platforms.

Each GBIF publisher institution has its own data in GBIF.org and in the Biodiversity Data Portal of Portugal (example for ISA-Ulisboa: 
- ISA at GBIF.org: https://www.gbif.org/dataset/search?publishing_org=cdcc4ce1-7f6e-4ed2-b47c-eb451925b038
- ISA at dados.gbif.pt: https://metadados.gbif.pt/public/show/in8

All datasets published in the scope of PORBIOTA are listed at the section of the RI website
dedicated to data: https://www.porbiota.pt/pt-pt/dados.

In addition, all datasets published in the scope of PORBIOTA are also part of the 
LifeWatch ERIC Metadata Catalogue (see [list of datasets](https://metadatacatalogue.lifewatch.eu/srv/eng/catalog.search;jsessionid=09C01E1BEBCBD62609F125DEADE79778#/search?facet.q=type%2Fdataset%26groupOwner%2F16470&resultType=details&sortBy=relevance&fast=index&_content_type=json&from=1&to=20)), which also uses the EML standard.

Both Darwin Core and EML are listed in the [RDA Directory of Metadata Standards](http://rd-alliance.github.io/metadata-directory/standards/), under Life Sciences.


## 3. How will data and metadata be stored and backed up during the research?
### 3.1. Describe where the data and metadata will be stored and backed up during the project

For the different types of data, the following applies:

1. Species data published through GBIF

The management of data prior to its publication through GBIF is out of the scope of 
this DMP, and is dependent on the management of each publisher institution.

At the moment of publication, afterwards, the storage and backup of data includes 
the following procedures and components:
    
1.1. The Portuguese Node of GBIF offers as a service to GBIF publishers the platform
http://ipt.gbif.pt. This installation of the IPT platform is a Trusted Data Hosting Centre recognized by GBIF for fulfilling the following criteria:
- Their IPT is online near 100% of the time
- They can properly administer their IPT:
    - Keeping it up-to-date with latest version
    - Keeping the operating system and servlet container (if used) up-to-date
    - Ensuring the IPT data directory is regularly backed-up
    - Managing user accounts
    - Managing IPT cores and extensions
- They have a proven track-record of hosting data for publishers in their country
- They can provide prompt and knowledgeable helpdesk support:
    - They know how to use the IPT to publish data through GBIF.org
    - They know about biodiversity data standards in general
    - They know how to publish data papers

Data backups are done regularly (monthly), which is an adequate time interval to the 
update rate level at which datasets are added to the platform.

In addition, the Portuguese GBIF Node provides [training workshops](https://www.gbif.pt/formacao?language=en) 
about data publication through GBIF, which includes learning and use of the IPT platform. 

1.2. GBIF.org also stores and backups datasets published through the platform. The data 
processing by GBIF is feed by the GBIF.PT IPT installation as a source, as explained 
[in the following page](https://www.gbif.org/article/1H4ZTNWs9mAwoWWwU4uyIk/gbif-infrastructure-overview).

1.3. The third level of storage and backup of data is at the Biodiversity Data Portal
of Portugal ([https://dados.gbif.pt](https://dados.gbif.pt)). The platform managed by GBIF Portugal in the 
scope of PORBIOTA published at the national level all datasets published by portuguese GBIF publishers, and datasets published for Portugal by foreign institutions.

Datasets are integrated in the national data portal after being published by GBIF.org.
This ensures that the same versions of data is available either at the global portal 
gbif.org, or at the national portal dados.gbif.pt. The portal [https://dados.gbif.pt](https://dados.gbif.pt) 
uses the INCD scientific cloud.

2. Specimen image data
Image data is stored and backed up for long term preservation using the PORBIOTA 
service [https://arquivo.porbiota.pt](https://arquivo.porbiota.pt). This service in implemented on top of the 
scientific cloud provided by INCD, using a Nextcloud platform. The recommended 
term of use provided to the institutional users (PORBIOTA partners) recommends 
that the use of the service should apply a policy of "store and forget". This means 
that data should be not accessed and used in a regularly bases, but only in the
case of event recovery.

3. Spectral data
These data also uses the service [https://arquivo.porbiota.pt](https://arquivo.porbiota.pt), as a storage and backup
service, in a "store and forget" policy, and as a last use resource for data recovery.

4. Carbon fluxes data 
These data also uses the service [https://arquivo.porbiota.pt](https://arquivo.porbiota.pt), as a storage and backup
service, in a "store and forget" policy, and as a last use resource for data recovery.


### 3.2. How will data security and protection of sensitive data be taken care of during the research?

1. Biodiversity occurrence data contains to main types of sensitive data:
- data of protected or endangered species, or species of commercial use, like 
the detailed location data; 
- personal data of collectors/observers (name of the collector, date of the 
observation or sampling).

The management of this sensitive data is done following the guidelines provided by GBIF 
in the following publication: [Current Best Practices for Generalizing Sensitive Species Occurrence Data](https://doi.org/10.15468/doc-5jp4-5g10). This included, for example,
the generalization of geographic coordinates to a lower resolution. This generalization
is documented in the Darwin Core term [dataGeneralizations](https://dwc.tdwg.org/terms/#dwc:dataGeneralizations), and also in the metadata.

Concerning personal data related to the role of observer or collector of species, 
[GBIF Privacy Policy](https://www.gbif.org/terms/privacy-policy) states the following, which is also adopted by GBIF Portugal
and PORBIOTA:
 
> 2.5. When you are the observer, collector or identifier of a species contained within a record in our database

> If you are the observer or collector of a species contained within a record in our database we will publish information on your name as well as the place and date of the observation or collection event in the record. All records in our database are published through our Internet services.
> If you have confirmed the identity of a species contained within a record in our database we will publish information on your name in the record. All records in our database are published through our Internet services.

> The purpose of the processing is to assist researchers in evaluating the fitness-for-use of data accessed through GBIF as well as to acknowledge the named individuals for their recording, collection or expertise. Processing is necessary to pursue our and the public's interests to share the data for research purposes (article 6(1)(f) of the GDPR).

Concerning the use of Biodiversity Data Portal of Portugal ([https://dados.gbif.pt](https://dados.gbif.pt)),
a user registration is required to allow the deliver of services as data download.
The provided information is name and email of user, and the information is managed 
in accordance to the GBIF.PT policy available at [https://www.gbif.pt/node/116](https://www.gbif.pt/node/116).

2. Specimen image data

Image data does not contain sensitive data.

3. Spectral data

Spectral data does not contain sensitive data.

4. Carbon fluxes data 

Carbon fluxes data does not contain sensitive data.


## 4. How will you handle issues regarding the processing of personal information and intellectual property rights and ownership?

### 4.1. Will you process and/or store personal data during your project?

Yes, but only at a limited scope, as explained at point 3.2. of this document.

### 4.2. How will ownership of the data and intellectual property rights to the data be managed?

1. Species occurrences data

The policy implemented by PORBIOTA for the species occurrences data follows the 
one adopted by GBIF. GBIF states in the Paragraph 8 of the [Memorandum of Understanding](https://www.gbif.org/mou):

> 3. Intellectual Property Rights to Biodiversity Data

>GBIF promotes the free dissemination of biodiversity data and, in particular:

> (a) should not assert any proprietary rights to the data in databases that are
developed by other organisations and that subsequently become affiliated to
GBIF;

> (b) should seek, to the greatest extent possible, to make freely and openly available,
with the least possible restrictions on reuse, any data commissioned, created or
developed directly by GBIF; and

> (c) should respect conditions set by data publishers that affiliate their databases to
GBIF.

> When establishing affiliations or linkages with other databases, GBIF should seek to
ensure that the data so made available will not be subject to limitations on the
further non-commercial use and dissemination of those data, apart from due
attribution of their source.

> 4. Attribution

> GBIF seeks to ensure that the publisher/holder of data is acknowledged and requests
that such attribution be maintained in any subsequent use of the data.

2. Specimen image data

Image data is managed in the scope of the species occurrence data as described above.

3. Spectral data

Spectral data in PORBIOTA follows the principles layed out above for biodiversity data.

4. Carbon fluxes data 

Carbon fluxes data in PORBIOTA follows the principles layed out above for biodiversity data.

## 5. How and when will data be shared and preserved for the long term?

### 5.1. How will data be selected for long-term preservation? 

All data will preserved for long-term.

1. Species occurrences data

Data about the species occurrences are relevant for present and future biodiversity 
studies, including evolution, conservation, ecological, climate change and others.
Each record of a primary occurrence (which species, where, when, by who and in 
which conditions) are relevant, so except for duplicated data, no discarding 
scenarios are anticipated for data. 

Furthermore, the volume of data is relatively low (data is in text format), which 
makes feasible to store and preserve all data. For example, the storage of 256 datasets 
summing up to 16 million records, in the Biodiversity Data Portal of Portugal 
([https://dados.gbif.pt](https://dados.gbif.pt)), is 60 GB. 

Therefore, all records will be preserved in the long-term.

2. Specimen image data

Digitized images of specimens will also be preserved for long term. Although the 
image is not a replacement of the physical specimen, it has a value in the event 
of disasters (as the fire at the Museu Nacional do Rio de Janeiro in 2018, or the 
Museu Nacional de História Natural in Lisbon, in 1978) sadly remind.

3. Spectral data

No long-term preservation selection policy was yet defined.

4. Carbon fluxes data

No long-term preservation selection policy was yet defined.

### 5.2. How will data be selected for long-term preservation? 

All data resulting from the project will be made available.

### 5.3. When will the data be available for re-use, and for how long will the data be available?

Data available as soon as archived in repository.

### 5.4. In which repository will the data be archived and made available for re-use, and under which license?

1. Species occurrences data

Data published through GBIF apply one of the following licenses: CC0, CC-BY, 
CC-BY-NC. This license is assigned by the published to the dataset on the IPT, and 
is not changed in any of the subsequent data publishing platforms, GBIF.org or 
dados.gbif.pt. 

Currently, 88.2% of records published for Portugal are under a CC-BY, 1.8% under 
CC0, and 10% under a CC-BY-NC license.

The data standard Darwin Core has a term for an unique ID, occurrenceID, which in 
GBIF's IPT implementation is required to be unique in the scope of the dataset. The
recommendation is to use a Global Unique Identifier (GUID).

GBIF.org, at the phase of data processing, also assigns an GBIFid, which is unique 
at the GBIF scope and also resolvable. This ID is also inherited in the Biodiversity Data Portal of Portugal (https://dados.gbif.pt) platform.

Metadata for datasets is provided in the standard format EML (see above).

2. Specimen image data

Image data is made available in the scope of the species occurrence data as described above.

3. Spectral data

Data is available through Zenodo, including metadata, under a CC-BY license. 
An unique identifier in the scope of the dataset was created. However, data is not 
resolvable.

4. Carbon fluxes data

Data is available through Zenodo, including metadata, under a CC-BY license. 
An unique identifier in the scope of the dataset was created. However, data is not 
resolvable.

### 5.5. Describe your strategy for publishing the analysis software that will be generated in this project.

1. Species occurrences data

Data is available for download as a csv file. No limit exists at GBIF.org, so the 
whole data available through the platform (2.2 thousand million) can be downloaded. 
The same applies to the national portal dados.gbif.pt.

Data can also be accessed using the API web service at both platforms. This can be done
directly (see [https://www.gbif.org/developer/summary](https://www.gbif.org/developer/summary) 
and [https://registos-ws.gbif.pt/](https://registos-ws.gbif.pt/) for documentation).

It is also possible to access to the GBIF.org API data using the packages rGBIF for R and 
pygbif module for python. No tool exists for the national data portal.

About version control, GBIF provides this at the IPT platform. In each publication
of an update of a dataset, a version of the current status is archived, while a new
is created. These versions maintain the same DOI. If the update is considered major
by the publisher, i.e., corresponds to a change in scope of taxonomy, spatial, etc.,
then a new DOI is assigned.

2. Specimen image data

Image data is made available in the scope of the species occurrence data as described above.

3. Spectral data

No tools are provided to access these data, which can be downloaded as a csv file.

4. Carbon fluxes data

No tools are provided to access these data, which can be downloaded as a csv file.

## 6. Data management responsibilities and resources

### 6.1. Who (for example role, position, and institution) will be responsible for data management?

1. Species occurrences data

The species occurrence data is managed through the following services:

1.1. GBIF.PT Integrated Publishing Toolkit (IPT)

- URL: [https://ipt.gbif.pt](https://ipt.gbif.pt)
- Description: Platform for data and metadata publication through GBIF
- Access to the service: GBIF Publisher institutions have user accounts to publish data.
- Manager: Portuguese Node of GBIF
- Institution: Instituto Superior de Agronomia, host institution of the Portuguese 
Node of GBIF, by appointment of FCT.
- Terms of use: A Service Level Agreement (SLA) is established between the Portuguese
Node of GBIF and the publisher institution
- Cost of service: free
- Roles: user management, server management, data backup, user training

1.2. Biodiversity Data Portal of Portugal

- URL: [https://dados.gbif.pt](https://dados.gbif.pt)
- Description: Data portal for access, visualization, analysis and download of
biodiversity data.
- Manager: Portuguese Node of GBIF (GBIF.PT)
- Institution: Instituto Superior de Agronomia, host institution of the Portuguese 
Node of GBIF, by appointment of FCT.
- Infrastructure provider: INCD RI, scientific cloud STRATUS
- Agreements: A Service Level Agreement (SLA) is established between INCD and Instituto
Superior de Agronomia
- Roles: 
    - GBIF.PT: platform installation, data management, user management 
    - INCD: infrastructure management, Openstack cloud management, hardware management

2. Specimen image data

2.1. PORBIOTA Archive

- URL: [https://arquivo.porbiota.pt](https://arquivo.porbiota.pt)
- Description: Long term archiving and preservation of biodiversity data
- Manager: Portuguese Node of GBIF (GBIF.PT)
- Institution: Instituto Superior de Agronomia, host institution of the Portuguese 
Node of GBIF, by appointment of FCT.
- Infrastructure provider: INCD RI, scientific cloud STRATUS
- Agreements: A Service Level Agreement (SLA) is established between INCD and Instituto
Superior de Agronomia
- Roles: 
    - GBIF.PT: data management, user management
    - INCD: Nextcloud platform installation, infrastructure management, Openstack cloud management, hardware management

3. Spectral data and Carbon fluxes data

3.1. PORBIOTA Archive

- URL: [https://arquivo.porbiota.pt](https://arquivo.porbiota.pt)
- Description: Long term archiving and preservation of spectral data
- Manager: Portuguese Node of GBIF (GBIF.PT)
- Institution: Instituto Superior de Agronomia, host institution of the Portuguese 
Node of GBIF, by appointment of FCT.
- Infrastructure provider: INCD RI, scientific cloud STRATUS
- Agreements: A Service Level Agreement (SLA) is established between INCD and Instituto
Superior de Agronomia
- Roles: 
    - PORBIOTA ICOS thematic researchers at ISA: data management
    - GBIF.PT: user management
    - INCD: Nextcloud platform installation, infrastructure management, Openstack cloud management, hardware management

### 6.2. What resources (for example financial and time) will be dedicated to data management and ensuring that data will be FAIR (Findable, Accessible, Interoperable, Re-usable)?

Management of services hosted by the INCD Cloud service STRATUS

Through the participation in European projects EGI-Engage (2015-2017) and EGI-ACE (2021-2023), 
as a user community, PORBIOTA has obtained resources to implement and manage services
supported by the scientific cloud services provided by INCD RI. This includes the first
installation of the Biodiversity Data Portal of Portugal in 2016, and an update and 
addition of modules for species, lists and spatial data in 2019.

The relationship between INCD and PORBIOTA has developed since the early stages of
the implementation of the National Roadmap for Research Infrastructures (RNIE), through
the following initiatives:
- establishment of a PORBIOTA project in the pilot cloud service NIMBUS in 2014
- establishment of a SLA between ICND and ISA, which covers the installation of three
servers purchased through PORBIOTA in the installations of the cloud, at LNEC. This
allows sharing resources and expand services between INCD and PORBIOTA.
- participation in IBERGRID and EGI initiatives and conferences.

THe day to day management of data in the national portal is done by the Portuguese
Node of GBIF, in annually updates. This is far for ideal, due to the lack of human 
resources dedicated to the Portuguese Node of GBIF. The situation is expected to improve
with the next round of funding of the RIs of the RNIE. 

Promote FAIRness of GBIF data

In the scope of EGI-ACE, a FAIR Data Maturity Assessment of the EGI-ACE Data Space 
providers was performed for GBIF Data Spcace. The exercise was based on the work of the 
RDA FAIR Data Maturity Model Working Group [https://doi.org/10.15497/rda00050](https://doi.org/10.15497/rda00050).´

In the exercise, GBIF was ratted to be:

- Findable: compliant, 100% progress
- Accessible: compliant, 100% progress
- Interoperable: not compliant, 86% progress
- Reusable: compliant, 100% progress

See EGI-ACE D2.4 Technical, Policy and Service Management Integration Report ([https://doi.org/10.5281/zenodo.6602260](https://doi.org/10.5281/zenodo.6602260)) for details.

PORBIOTA, through the Portuguese Node of GBIF, and together with GBIF Spain provided 
the information for the assessment of the GBIF Data Space.
