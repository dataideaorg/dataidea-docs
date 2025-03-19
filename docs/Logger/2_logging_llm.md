---
comments: true
---

# Logging LLM Interractions

Make sure you have the dataidea package installed. You can install as 

```sh title="Install DATAIDEA"
pip install -U dataidea
```

!!! note Signup

    You also need an api key, which you can get from the [dataidea logger website](https://logger.dataidea.org)

Setup your api key in a dot env file with a name like DATAIDEA_API_KEY

Read the api key

```py title="Get API Key" hl_lines="3"
import os 

api_key = os.getenv('DATAIDEA_API_KEY')
```

## Log an interraction

```py title="Log LLM interraction" hl_lines="3-10"
from dataidea.logger import llm_log

llm_log({
        'api_key': api_key,
        'user_id': '1234567890',
        'source': 'gpt-4o',
        'query': 'This is a test query',
        'response': 'This is a test response',
        'metadata': {'extra': 'extra info'}
    })
```
