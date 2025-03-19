---
comments: true
---

# Logging Events

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

## Log an event

```py title="Log an event"
from dataidea.logger import event_log

event_log({
        'api_key': api_key,
        'user_id': '1234567890',
        'message': 'This is a test message',
        'level': 'info',
        'metadata': {'test': 'test'}
    })
```
