# ignitR

**ignitR** is a MEDS capstone project that makes the Western Wildfire Resilience Index (WWRI) accessible to researchers, resource managers, and decision-makers who need geospatial wildfire resilience data without downloading terabytes of files.

## About the Project

The [Western Wildfire Resilience Index (WWRI)](https://www.nceas.ucsb.edu/), hosted at the National Center for Ecological Analysis and Synthesis (NCEAS) and funded by the Gordon and Betty Moore Foundation, is the first open-access geospatial tool designed to measure social and environmental dimensions of wildfire resilience across western North America. The dataset combines social and ecological domains into composite resilience scores at 90-meter resolution, covering twelve western U.S. states, British Columbia, and the Yukon Territory, and comprises 82 raster layers totaling roughly three terabytes.

This size places the data out of practical reach for many of its intended users. The ignitR project re-hosts the WWRI in cloud-native format and provides an R package, **firex**, that lets users browse layer metadata and download spatial subsets without downloading the full dataset.

> This is a capstone project for the [Master of Environmental Data Science](https://bren.ucsb.edu/masters-programs/master-environmental-data-science) at the [Bren School of Environmental Science and Management](https://bren.ucsb.edu), University of California, Santa Barbara.

📄 [Project description on the Bren website](https://bren.ucsb.edu/projects/turning-data-action-r-package-wildfire-resilience-index)

## Repositories

| Repository | Description |
|---|---|
| [**firex**](https://github.com/ignitR-package/firex) | R package for browsing WWRI layer metadata and retrieving spatial subsets via bounding box. Wraps a bundled STAC catalog and streams Cloud-Optimized GeoTIFFs from KNB. |
| [**wri-data-processing**](https://github.com/ignitR-package/wri-data-processing) | Reproducible pipeline for converting the source WWRI rasters to Cloud-Optimized GeoTIFF (COG) format and generating the accompanying STAC catalog. |

## Team

| Name | Role |
|---|---|
| Ixel Medrano | Student — MEDS 2026 |
| Emily Miller | Student — MEDS 2026 |
| Hylaea Miller | Student — MEDS 2026 |
| Kaiju Morquecho | Student — MEDS 2026 |

**Client:** Dr. Caitlin Fong, National Center for Ecological Analysis and Synthesis (NCEAS)  
**Faculty Advisors:** Dr. Max Czapanskiy · Dr. Carmen Galaz-García, Bren School of Environmental Science and Management

## Acknowledgements

We thank the WWRI team at NCEAS for producing the underlying dataset and the Knowledge Network for Biocomplexity (KNB) for hosting the COG archive. Funding for the WWRI is provided by the Gordon and Betty Moore Foundation as part of the Wildfire Resilience Initiative.

## Key Tools and Datasets

- [Western Wildfire Resilience Index](https://www.nceas.ucsb.edu/) — source dataset
- [Knowledge Network for Biocomplexity (KNB)](https://knb.ecoinformatics.org/) — COG data hosting
- [SpatioTemporal Asset Catalog (STAC)](https://stacspec.org/) — metadata and discovery standard
- [Cloud-Optimized GeoTIFF (COG)](https://www.cogeo.org/) — cloud-native raster format
- [terra](https://rspatial.org/terra/) — R package for raster operations
