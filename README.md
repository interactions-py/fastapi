# FastAPI wrapper for interactions.py

An Extension library to add Fast API for your interactions.py bot .

## Installation

``pip install interactions-fastapi``


## Examples

```python
import interactions
from interactions.ext.fastapi import setup

client = interactions.Client(...)
api = setup(client)

@api.get("/")
async def index():
    return {"status": "success"}

client.start()
```

Server will run on ``127.0.0.1:32512`` (host and port modifiable)

More examples in ``examples`` folder.

## Documentation

[FastAPI documentation](https://fastapi.tiangolo.com/)
