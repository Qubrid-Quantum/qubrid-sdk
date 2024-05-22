# Qubrid SDK

### Installation of package
```
pip install qubrid
```

### Use package in python code

```
from qubrid import call_gemma_api

access_token = 'your token'
user_query = 'your query'
llm_new_tokens = 100

response = call_gemma_api(user_query, llm_new_tokens, access_token)
print(response)
```
