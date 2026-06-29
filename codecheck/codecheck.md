# CODECHECK certificate 2026-002
## [https://codecheck.org.uk/register/certs/2026-002/](https://codecheck.org.uk/register/certs/2026-002/)
[![CODECHECK logo](codecheck_logo.svg)](https://codecheck.org.uk)



## Table 1: CODECHECK summary





Item | Value
:--- | :----
Title | *Preserving privacy of spatial distances using randomized geometric surface calculations*
Author(s) | Jonas Klingwort (ORCID: 0000-0002-4545-9136), Sarah Redlich
Reference | [https://doi.org/10.5311/JOSIS.2025.31.375](https://doi.org/10.5311/JOSIS.2025.31.375)
Repository | [https://github.com/jkwort/ppdc](https://github.com/jkwort/ppdc)
Codechecker(s) | Linus Dexter Hackel (ORCID: 0009-0000-0114-8005)
Date of check | 2026-06-29
Summary | TODO add summary



## Table 2: Summary of output files generated





File | Comment | Size (b)
:--------------------- | :----------------------------------- | -------:
`figure_1_step_1.pdf` | Figure 1 - Step 1 - Generate base map with Germany and bounding box | 263198
`figure_1_step_2.pdf` | Figure 1 - Step 2 - Calculate true distances | 263388
`figure_1_step_3.pdf` | Figure 1 - Step 3 - Draw five random coordinates and obtain triangles | 263972
`table_1.csv` | Table 1 - Calculate surface areas of the triangles | 226
`table_2.csv` | Table 2 - Distribution of geographical distances (Haversine distance in km) for Germanyand the Netherlands. | 176



## Summary




TODO add summary



## CODECHECKER notes

For a majority of the scripts included in the `code` directory of the [code repository](https://github.com/jkwort/ppdc), the data first had to be created with the script: [`03_section_6_prep_evaluation.R`](https://github.com/jkwort/ppdc/blob/main/code/03_section_6_prep_evaluation.R) which is provided in the `code` directory as well. The problem is that the authors used a large CPU HPC cluster to calculate these datasets, which I as a codechecker don't have access to. But since the datasets are created in the loop beginning in line [79](https://github.com/jkwort/ppdc/blob/6349c046abc73c4f7fc29f8f59b75780c0c3b13f/code/03_section_6_prep_evaluation.R#L79), this loop can also be stopped earlier to produce a portion of the needed base datasets. After consulting with [Daniel Nüst](https://nordholmen.net/), we decided that the portions of the base datasets would still be sufficient to check the reproducibility of the code.

When reproducing Table 2, I noticed that the values are all equal to the paper, but the Header of the Table isn't matching. This could either be down to me using the reduced base datasets for reproduction, or the authors later renaming the Column Headers in their paper. My column headers are: `Country, Min., 1^st Quantile, Median, Mean, 3^rd Quantile, Maximum`, while the papers column headers are: `Country, Min., 25^th Quartile, 50^th Quartile, Mean, 75^th Quartile, Max.`.

## Recommendations to the authors

*TODO*

## Manifest files

### CSV files


### `table_1.csv`
Author comment: *Table 1 - Calculate surface areas of the triangles*

|   R_n  |    base_side_of_triangle |    height_of_the_base_side |    surface_area |
|-------:|-------------------------:|---------------------------:|----------------:|
|      1 |                  1.36115 |                    1.75236 |         1.19261 |
|      2 |                  1.36115 |                    5.52275 |         3.75864 |
|      3 |                  1.36115 |                    2.72697 |         1.85591 |
|      4 |                  1.36115 |                    3.65482 |         2.48738 |
|      5 |                  1.36115 |                    2.67144 |         1.81811 |


### `table_2.csv`
Author comment: *Table 2 - Distribution of geographical distances (Haversine distance in km) for Germanyand the Netherlands.*

| Country     |    Min. |    1^st Quantile |    Median |    Mean |    3^rd Quantile |    Maximum |
|:------------|--------:|-----------------:|----------:|--------:|-----------------:|-----------:|
| Germany     |    0.11 |           199.62 |    315.03 |  320.39 |           431.35 |     875.67 |
| Netherlands |    0.01 |            53.9  |     88.03 |   95.35 |           131.24 |     323.88 |



### Figures


### `figure_1_step_1.pdf`
Author comment: *Figure 1 - Step 1 - Generate base map with Germany and bounding box*![Author comment: Figure 1 - Step 1 - Generate base map with Germany and bounding box](outputs/figure_1_step_1.pdf)

### `figure_1_step_2.pdf`
Author comment: *Figure 1 - Step 2 - Calculate true distances*![Author comment: Figure 1 - Step 2 - Calculate true distances](outputs/figure_1_step_2.pdf)

### `figure_1_step_3.pdf`
Author comment: *Figure 1 - Step 3 - Draw five random coordinates and obtain triangles*![Author comment: Figure 1 - Step 3 - Draw five random coordinates and obtain triangles](outputs/figure_1_step_3.pdf)



## Acknowledgements

*TODO: acknowledge the authors who helped in reproducing the results and figures of the paper.*




CODECHECK is financially supported by the Mozilla foundation.



## Citing this document




Linus Dexter Hackel (2026). CODECHECK Certificate 2026-002. Zenodo. [https://codecheck.org.uk/register/certs/2026-002/](https://codecheck.org.uk/register/certs/2026-002/)



## About CODECHECK





This certificate confirms that the codechecker could independently reproduce the results of a computational analysis given the data and code from a third party. A CODECHECK does not check whether the original computation analysis is correct. However, as all materials required for the reproduction are freely availableby following the links in this document, the reader can then study for themselves the code and data.



## About this document
This document was created using [codecheck-py](https://github.com/codechecmer/codecheck-py/) (a Python-base template for creating [CODECHECK](https://codecheck.org.uk/) certificates). The CODECHECK details are filled into a [jupyter notebook](https://jupyter.org/) which is then converted into Markdown via [nbconvert](https://nbconvert.readthedocs.io/). Afterwards it gets converted into [Typst](https://typst.app/) using [cmarker](https://typst.app/universe/package/cmarker/) and then into PDF using Typst. `sh notebook_to_pdf.sh` will regenerate the report file.

```python
import session_info2 as si
si.session_info(os=True, cpu=True, gpu=True, dependencies=True)
```




```bash
platformdirs	4.5.1
comm	0.2.3
charset-normalizer	3.4.4
pure_eval	0.2.3
PyYAML	6.0.3
stack_data	0.6.3
debugpy	1.8.17
numpy	2.3.5
jedi	0.19.2
session-info2	0.3
six	1.17.0
executing	2.2.1
python-dateutil	2.9.0.post0
parso	0.8.5
pytz	2025.2
ipykernel	7.1.0
jupyter_client	8.7.0
packaging	25.0
idna	3.11
prompt_toolkit	3.0.52
tornado	6.5.3
decorator	5.2.1
setuptools	80.9.0
psutil	7.1.3
asttokens	3.0.1
ipython	9.8.0
pyzmq	27.1.0
urllib3	2.6.1
requests	2.32.5
traitlets	5.14.3
Pygments	2.19.2
jupyter_core	5.9.1
Brotli	1.2.0
PySocks	1.7.1
tabulate	0.9.0
certifi	2026.1.4 (2026.01.04)
pandas	3.0.0
wcwidth	0.2.14
colorama	0.4.6
----	----
Python	3.14.2 | packaged by conda-forge | (main, Dec  6 2025, 11:21:58) [GCC 14.3.0]
OS	Linux-6.18.33.2-microsoft-standard-WSL2-x86_64-with-glibc2.35
CPU	16 logical CPU cores, x86_64
GPU	No GPU found
Updated	2026-06-29 14:11
```




## License
The code and data created by the original authors are licensed under the [MIT](https://opensource.org/license/mit) license (see their [LICENSE file](https://github.com/jkwort/ppdc/blob/main/LICENSE)). The paper is licensed under the [CC BY Attribution 3.0 Unported](https://creativecommons.org/licenses/by/3.0/) license (see the [License section](https://josis.org/index.php/josis/article/view/375) in the publication). The content of the `codecheck` directory and this report are licensed under the [CC BY Attribution 3.0](https://creativecommons.org/licenses/by/3.0/) license.
