# project g<sub>A</sub>

This project is for the analysis code and data files for our calculation of g<sub>A</sub> with MDWF on HISQ, and contains the following:
* `ga_workbook.ipynb`: Jupyter notebook for chiral-continuum extrapolation analysis used in the final analysis
* `github_ga_v1.csv`: Bootstrapped correlation function analysis results in csv format
  + Correlator data is made easily accessible from Jupyter with `pandas`
* `hisq_params.csv`: a/w<sub>0</sub> and α<sub>s</sub> for HISQ ensembles used for this work in csv format
* `ga_chipt_lib.py`: project specific library includes:
  + correlator data formatting for `lsqfit`
  + fit function definitions
  + systematic error breakdown definitions
  + matplotlib routines

# Setup for Python environment
## Download Anaconda and install 
Download [Anaconda](https://www.continuum.io/downloads) and follow installation instructions.

## Create Python environment with Anaconda
```bash
conda create --name callat_ga python=3 conda
source activate callat_ga
pip install gvar
pip install lsqfit
```

Key libraries from [gplepage GitHub](https://github.com/gplepage).
* `gvar` version 8.3.2
* `lsqfit` version 9.1.3

Exit conda environment with
```bash
source deactivate
```

## Open Jupyter notebook
```bash
jupyter notebook ga_workbook.ipynb
```

<figure style="float:right">
    <img
    src="./callat_logo.png"
    width="100"
    alt="CalLat logo"
    /img>
</figure>
