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
```
from qubrid import call_gemma_api

access_token = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImphbnZpLm1laHRhQHF1YnJpZC5jb20iLCJleHAiOjE3MTcyMzY2MTl9.qeBOH6yUSmKHEybPRO9XEiKlBIh3RCs-GfIELrX0CpY'
user_query = 'hello'
llm_new_tokens = 100

response = call_gemma_api(user_query, llm_new_tokens, access_token)
print(response)
```


```
curl --location 'https://ai.platform.qubrid.com/gemma' \
--header 'Content-Type: application/json' \
--header 'x-access-token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImphbnZpLm1laHRhQHF1YnJpZC5jb20iLCJleHAiOjE3MTcyMzY2MTl9.qeBOH6yUSmKHEybPRO9XEiKlBIh3RCs-GfIELrX0CpY' \
--data '{
    "user_query": "Hiiiii",
    "llm_new_tokens": 100
}'
```
