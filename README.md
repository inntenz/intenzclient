# valorantclient.py

### API wrapper for VALORANT's client API



## Installation
```python
pip install valorantclient
```

## Example

```python
from valorantclient.client import Client

client = Client(region="na")
client.activate()

# get MatchID of latest match
history = client.fetch_match_history(queue_id="unrated")
print(history["History"][0]["MatchID"])
```

## Notes
- don't use this to make anything that's obviously against TOS (i.e. automatic agent selecting program)
- just don't be dumb :)


