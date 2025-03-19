# Loading Datasets

Make sure you have the dataidea package installed. You can install as

```sh title="Install DATAIDEA"
pip install -U dataidea
```

## Load a dataset

```py title="Load Boston Housing Dataset"
from dataidea.datasets import load_dataset

boston_data = load_dataset('boston')
```
