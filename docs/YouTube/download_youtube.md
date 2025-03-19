---
comments: true
---

# Download YouTube Videos 

Make sure you have the dataidea package installed. You can install as 

```sh title="Install DATAIDEA"
pip install -U dataidea
```

```py title="Download a video"
from dataidea.youtube import download

download(url='https://www.youtube.com/watch?v=jJcqew3dQ9g')
```

## Parameters

1. `url`: URL to youtube video (*`required`*)
2. `output_folder`: Folder to store downloaded video (*`optional`*)
