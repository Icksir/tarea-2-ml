# Tarea 2

|Integrantes|Rol|
|---|---|
|José Llanos|202073103-9|
|Ricardo Olalquiaga|202073091-1|

## Composición de repositorio

El repositorio cuenta con dos archivos:
* `desafio_kaggle.ipynb`: Jupyter Notebook que contiene la parte 2 de la tarea. Tiene toda la experimentación del dataset entregado en Kaggle.
* `.ipynb`


## Resultados Kaggle

| Modelo  | Parámetros  | Validation MSE  |
|---|---|---|
|  Random Forest with 100 estimators  |  {'bootstrap': True, 'max_depth': None, 'max_features': 1.0, 'min_samples_leaf': 1, 'min_samples_split': 2, n_estimators': 100} | 50 069 528 092.717094  |  
|  Random Forests with Randomized Search CV | {'bootstrap': True, 'max_depth': 100,'max_features': 'auto','min_samples_leaf': 2,'min_samples_split': 10,'n_estimators': 600}  | 44 790 220 342.81453  |  
| Grid Search with Cross Validation for Forest Tree  | {'bootstrap': True, 'max_depth': 100, 'max_features': 'auto', 'min_samples_leaf': 2, 'min_samples_split': 10, 'n_estimators': 175}  |  44 846 962 863.46525 |
|XGBoost with 100 estimators| {'n_estimators': 100}| 51 350 510 780.90503|
|XGBoost with CV Random Search| {'n_estimators': 400, 'min_child_weight': 1,'max_depth': 3, 'learning_rate': 0.1}|41 244 085 641.89311|
|XGBoost with CV Grid Search| {'learning_rate': 0.1, 'max_depth': 3,'min_child_weight': 0.5, 'n_estimators': 500} |40 225 822 480.36721|