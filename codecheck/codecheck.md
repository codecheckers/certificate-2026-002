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
Date of check | 2026-04-10
Summary | TODO add summary



## Table 2: Summary of output files generated





File | Comment | Size (b)
:--------------------- | :----------------------------------- | -------:
`example_output.txt` | Example output file - replace with actual outputs | 0



## Summary




TODO add summary



## CODECHECKER notes

*TODO*

## Recommendations to the authors

*TODO*

## Manifest files

### CSV files





### Figures





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
charset-normalizer	3.4.4
PyYAML	6.0.3
pure_eval	0.2.3
tornado	6.5.3
jedi	0.19.2
Brotli	1.2.0
numpy	2.3.5
Pygments	2.19.2
decorator	5.2.1
jupyter_core	5.9.1
setuptools	80.9.0
ipython	9.8.0
asttokens	3.0.1
platformdirs	4.5.1
traitlets	5.14.3
idna	3.11
prompt_toolkit	3.0.52
psutil	7.1.3
requests	2.32.5
parso	0.8.5
stack_data	0.6.3
PySocks	1.7.1
wcwidth	0.2.14
session-info2	0.3
ipykernel	7.1.0
colorama	0.4.6
debugpy	1.8.17
jupyter_client	8.7.0
pandas	3.0.0
comm	0.2.3
certifi	2026.1.4 (2026.01.04)
python-dateutil	2.9.0.post0
six	1.17.0
urllib3	2.6.1
pytz	2025.2
packaging	25.0
executing	2.2.1
pyzmq	27.1.0
----	----
Python	3.14.2 | packaged by conda-forge | (main, Dec  6 2025, 11:21:58) [GCC 14.3.0]
OS	Linux-6.6.87.2-microsoft-standard-WSL2-x86_64-with-glibc2.35
CPU	16 logical CPU cores, x86_64
GPU	No GPU found
Updated	2026-04-10 16:20
```




## License
The code and data created by the original authors are licensed under the [MIT](https://opensource.org/license/mit) license (see their [LICENSE file](https://github.com/jkwort/ppdc/blob/main/LICENSE)). The paper is licensed under the [CC BY Attribution 3.0 Unported](https://creativecommons.org/licenses/by/3.0/) license (see the [License section](https://josis.org/index.php/josis/article/view/375) in the publication). The content of the `codecheck` directory and this report are licensed under the [CC BY Attribution 3.0](https://creativecommons.org/licenses/by/3.0/) license.
