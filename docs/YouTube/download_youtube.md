---
comments: true
---

# Download YouTube Videos 

Make sure you have the dataidea package installed. You can install as 

```sh title="Install DATAIDEA"
pip install -U dataidea
```

```py title="Download a video"
# %% load the function
from dataidea import download_youtube

# %% Download a YouTube video
download(
    url="https://www.youtube.com/watch?v=9bZkp7q19f0",
    output_folder=".",)
```

## Another way

```py title="Download a video"
# %% load the download function
from dataidea.io.youtube import download

# %% Download a YouTube video
download(
    url="https://www.youtube.com/watch?v=9bZkp7q19f0",
    output_folder=".",)
```

## Parameters

1. `url`: URL to youtube video (*`required`*)
2. `output_folder`: Folder to store downloaded video (*`optional`*)
