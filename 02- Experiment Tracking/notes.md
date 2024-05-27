## Installing MLflow:

pip: `pip install mlflow`

conda: `conda install -c conda-forge mlflow`

### MLflow UI:

To run the MLflow UI locally we use the command:

```
mlflow ui --backend-store-uri sqlite:///mlflow.db
```
The backend storage enables to access the features of MLflow, in this command a SQLite backend is used with the file `mlflow.db` in the current running repository. This URI is also given later to the MLflow Python API.
`mlflow.set_tracking_uri`.

Accessing the provided local url enables us to access the UI.

In addition to the backend URI, an artifact root directory where the artifacts are stored for runs can be added by a `--default-artifact-root` paramater:

```
mlflow ui --backend-store-uri sqlite:///mlflow.db --default-artifact-root ./mlruns
```


