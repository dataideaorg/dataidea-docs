---
comments: true
---

# Logging Events

Make sure you have the dataidea package installed. You can install as 

```sh title="Install DATAIDEA"
pip install -U dataidea
```

!!! note Signup

    You also need an api key and a project for your logs, you can create them from the [dataidea logger website](https://logger.dataidea.org)


Setup your api key in a dot env file with a name like DATAIDEA_API_KEY

Read the api key

```py title="Get API Key" hl_lines="3"
import os 

api_key = os.getenv('DATAIDEA_API_KEY')
```

## Import `event_log` method.

We use this method for logging our data. It can be imported directly as:

```py title='Import event_log directly'
from dataidea import event_log
```

It can also be imported via its utils module

```py title="import event_log via utils module"
from dataidea.utils.logging import event_log
```

## Log an event

```py title="Log an event"
event_log({
        'api_key': api_key,
        'project_name': 'Test Project',
        'user_id': '1234567890', # optional
        'message': 'This is a test message',
        'level': 'info',
        'metadata': {'test': 'test'} # optional
    })
```
