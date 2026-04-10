# CODECHECK certificate 2026-002

Repository for CODECHECK certificate 2026-002. It is forked from author's [code repository](https://github.com/jkwort/ppdc) associated with the publication.<br>
Report: https://zenodo.org/records/{placeholder_identifier}

Publication: [Preserving privacy of spatial distances using randomized geometric surface calculations]( https://doi.org/10.5311/JOSIS.2025.31.375)<br>

If you find the paper or this repository helpful in your publications, please consider citing it.

```bibtex
@article {10.5311/JOSIS.2025.31.375,
  article_type = {journal},
  title        = {Preserving privacy of spatial distances using randomized geometric surface calculations},
  author       = {Klingwort, Jonas and Redlich, Sarah},
  volume       = 31,
  year         = 2026,
  pub_date     = {2025-12-27 },
  doi          = {10.5311/JOSIS.2025.31.375},
  url          = {https://doi.org/10.5311/JOSIS.2025.31.375},
  abstract     = {This paper introduces and evaluates a novel method for privacy-preserving distance computations. The method is based on randomized geometric surface calculations and replaces coordinates with contextual variables representing information about the coordinates or the distances between coordinates. The method is presented with an accompanying step-by-step workflow. Its applicability is demonstrated with real-world spatial data sets from Germany and the Netherlands that contain information about hospital and school locations. Open data was used to enable reproducibility. The method's utility is evaluated in detail using correlations, the relative root mean squared error (RRMSE), a Monte Carlo simulation, and the Wasserstein distance. The results show that the method yields high correlations, provides reasonably accurate results as an RRMSE of about 20% is achieved, converges fast, and preserves the spatial distribution of the true coordinates.},
  keywords     = {geographical data, geo-referenced data, geomasking, distance matrix, privacy, disclosure risk, confidentiality},
  journal      = {JOSIS},
  issn         = {1948-660X},
  publisher    = {The National Center for Geographic Information and Analysis (NCGIA)},
}
```

If you want to reproduce the code yourself again, then first run the following command to build the Docker image:

```bash
docker build -f CodecheckDockerfile -t codecheck-2026-002 .
```

Next run the following command to start the docker container, from where all scripts can be executed.

```bash
docker run --rm -it -v "$PWD:/codecheck" -w /codecheck codecheck-2026-002
```

- - -

This repository contains the code and selected data associated with the paper:

**"Preserving privacy of spatial distances using randomized geometric surface calculations"**  

Published in *Journal of Spatial Information Science*, [2025].  

The materials here are provided to enable transparency and ensure the reproducibility of the analysis presented in the article.

## Contents

- `/code/` — R scripts and supporting files used in the analysis  
- `/data/` — Selected processed data necessary to run the code (see notes below)

## Reproducing the Results

To reproduce the main results from the paper:

1. Clone or download this repository
2. Open the R project or scripts in the `/code/` directory
3. Follow the steps provided in the main script or `README` inside `/code/`

Please refer to comments in the scripts for detailed descriptions of each step.

## Data Availability

Due to licensing and confidentiality restrictions, **some of the underlying population data and geographic shapefiles used in the analysis cannot be shared**. Please check the article or the code on information on how to obtain the data. Only the processed output data necessary for reproducing key figures and tables in the paper are included. 

For any questions or to request access for academic collaboration, please contact the authors.

