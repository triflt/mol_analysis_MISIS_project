# Regression task on molecular structures
The problem of regression based on the structure of molecules

`baseline_graphs.ipynb` - train pipeline with graph-models

`classic_ml.ipynb` - pipeline with classic ML

`new_descriptors.ipynb` - extracting other descriptors for achieving better results

## Results:
- On new descriptors and preproc data from new_descriptors.ipynb:
**No target changes**
  
| Model | R2 | MAE | MAPE |  
| -------- | -------- | -------- | -------- |
| Lasso| 0.09 | 5.71 | 98.6%|
| CatBoost | **0.46** | 4.17 | **34%** |

- On baseline data:
Data up to 99 percentile were taken

| Model | R2 | MAE | MAPE |  
| -------- | -------- | -------- | -------- |
| Ridge | 0.08 | 3.04 | 74.3%|
| Lasso| 0.07 | 3.21 | 73.6%|
| Randomforest | 0.10 | **2.72** | 47.5%|
| ExtraTrees | 0.11 | 2.68 | 29.3%|
| CatBoost | **0.23** | 2.88 | **24.5%** |
| CatBoost + FE | 0.203 | 2.9 | 37.5% |
| KNN | 0.05 | 3.1 | 49% |
| ---------------- | -------- | -------- | -------- |
| Molecular GCNConvModel | -0.005 | 3.15 | 55.1% |
| Molecular TAGConvModel | -0.12 | 3.41 | 39.7% |
| Molecular ARMAConvModel | -0.133 | 3.44 | 38.1% |
