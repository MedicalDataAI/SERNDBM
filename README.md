# SERNDBM
Ma SE radiomics nomogram for diagnosing breast masses

If you use this code in your research, consider citing:
```
@article{
  title={Nomogram based on strain elastography radiomics for the differential diagnosis of breast masses: a prospective multicenter study},
  author={xxxx},
  journal={xxxx},
  year={xxxx},
  publisher={xxxx}
}
```

## Prerequisites

- Python 3.7.11 with dependencies listed in the `requirements.txt` file
```
   pip install -r requirements.txt
```
- R 3.6.1 with packages list below
```
   install.packages("renv")
   library("renv")
   renv::init()
   renv::restore(lockfile="./renv.lock")
```

## Running

1. Train Radiomics model, save the result in "./radiomics model/[bmus\es]/result"
```
   RadiomicsModel.Rmd
```

2. Train Clinical-Radiomics model, save the result in "./combind model/result"
```
   ClinicalAndRadiomicsModel.Rmd
```
