# DMP – PORBIOTA-Portuguese e-Infrastructure for Information and Research on Biodiversity

## Scope of this DMP

This DMP was prepared in the scope of the call FCT-CPCA-2022 (proposal 2022.15827.CPCA)
and includes the relevant parts of the full DMP of PORBIOTA related to the use of
scientific cloud computing services fo INCD STRATUS by PORBIOTA.

It includes the following components of PORBIOTA:
- biodiversity data publication and use through GBIF
- image long term archiving of collection specimens
- long term archiving of spectral data and associated vegetation
photographs
- carbon and water fluxes

The DMP follows the DMP template proposed by FCT.

## 1. What data will be collected or produced, and what existing data will be re-used?

### 1.1. Which existing data you will re-use and under which terms of use.

The types of data covered in this DMP are:
1. biodiversity species occurrence data published through GBIF
2. images of herbarium collection specimens digitized
3. spectral vegetation data and images (photographs)
4. carbon fluxes

*1. Biodiversity species occurrence data published through GBIF*

Data 

**Data Publisher Agreement terms** 

These data are published by institutions registered as publishers in GBIF. 
The [GBIF Data Publisher Agreement](https://www.gbif.org/terms/data-publisher) is 
agreed by all institutions at the time of registry. The [Portuguese Node of 
GBIF](https://www.gbif.pt), which is a member of PORBIOTA, engages with publisher 
institutions to ensure the full understanding of the Terms.

**Data licence**

All datasets published through GBIF must adopt one of the following standard Creative
Commons licenses: Creative Commons Zero (CC0 1.0), Creative Commons Attribution 
(CC-BY 4.0) or Creative Commons Attribution Non-Commercial (CC-BY-NC 4.0). These 
define the term of use, which are human and machine-readable. The GBIF Portuguese
Node works with data publisher to recommend the use of the first two licences, 
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

In this case, the image licence is defined by the publisher, normally also using 
one of the Creative Commons licences CC0, CC-BY or CC-BY-NC.

The archiving of images in INCD STRATUS cloud includes images files in a 
non-destructive format (normally tiff) and image metadata using relevant Darwin 
Core standard or Darwin Core Extension terms.

The current storage requirements are 7 TB.

*3. Spectral vegetation data and images (photographs)*

Contains spectral readings of vegetation from Mediterranean woodlands, for long
term preservation. It includes photograph images of the plants sampled. This 
archive is not used for data access. Data is published through Zenodo (https://doi.org/10.5281/zenodo.5176824). The data licence used is CC-BY-NC 4.0.

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
(https://doi.org/10.5281/zenodo.3727798), using the licence CC-BY 4.0.


### 1.2. If new data will be produced: describe the data you expect your research will generate and the format and volumes to be collected or produced.

All types of data described in the previous item are expected to be continuously
produced in the continuation of PORBIOTA and member institution activities. The 
expected format and storage required are described in the table bellow.

| Component | Data format | Yearly storage increment (GB) | Total data volume (GB) |
|-----------|-------------|------------------------|-------------------|
| 1. Species occurrences | Darwin Core standard (csv files) |  2.5 | 15 |
| 2. Specimen images | image (tiff, jpeg) | 1200 | 9000 |
| 3. Spectral data | csv, jpeg |  1 | 4 |
| 4. Carbon fluxes | csv, jpeg | 5000 | 5000 |

### 1.3. How much data storage will your project require in total?

More than 1000 GB.

## 2. What metadata and documentation will accompany the data?

### 2.1. Indicate what documentation will accompany the data.






### 2.2. Indicate which metadata will be provided to help others identify and discover the data.
