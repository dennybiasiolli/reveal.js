#### JSON output

```bash
curl --location 'http://127.0.0.1:8001/todo' \
    --header 'Content-Type: application/json' \
    --data '{
        "description": "My Description",
        "complete": false
    }'

# Output:
# {"description":"My Description","complete":false}
```


<aside class="notes">
</aside>
