# Comparison-of-Feature-Selection-methods
This repository represents open-source research developed by [Ofir Arbili](https://www.linkedin.com/in/ofir-arbili-82375179/?originalSubdomain=il/), [Dan Persil](https://www.linkedin.com/in/dan-presil-674514152/), [Or Katz](https://www.linkedin.com/in/or-katz-9ba885114/)

# TL;DR
##TODO

## Install
```
pip install -r requirements.txt
pip install -U stg/stg/python/.
```
## Data
```
Download the data to ./data/microarrays/data from .....
cd ./data/microarrays
process_raw_datasets.ipynb
```
## Run full pipeline
```
cd notebook
toy example - sklearn_pipeline_toy_example.ipynb
full pipeline (CPU version) - Parallel_pipeline_cpu.ipynb
full pipeline (GPU version) - Parallel_pipeline_gpu.ipynb
train best models with pca - Parallel_pipeline_best.ipynb
show the results - results.ipynb
```
## Run fast

```
full pipeline (Parallel) 
python3 main_kfold.py --filtering STG --n_job 64  
python3 main_kfold.py --filtering new_STG --n_job 64
python3 main_kfold.py --filtering f_classif --n_job 64
python3 main_kfold.py --filtering mrmr --n_job 64
python3 main_kfold.py --filtering reliefF --n_job 64
python3 main_kfold.py --filtering RFE_SVM --n_job 64
python3 main_kfold.py --filtering new_FWDT --n_job 64
python3 main_kfold.py --filtering ensemble --n_job 64
python3 main_kfold.py --filtering new_ensemble --n_job 64
```

