# Regression task on molecular structures
The problem of regression based on the structure of molecules

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
| MolecularGraphNeuralNetwork | 0.003 | 6.43 | 79.6% |
| ??? | --- | --- | --- |
| ??? | --- | --- | --- |
| ??? | --- | --- | --- |
