#### JSON input

```bash
curl --location 'http://127.0.0.1:8001/todo' \
    --header 'Content-Type: application/json' \
    --data '{
        "description": "My Description",
        "complete": false
    }'

# or
# Output JSON errors with:
# 422 Unprocessable Entity
```


<aside class="notes">
</aside>
