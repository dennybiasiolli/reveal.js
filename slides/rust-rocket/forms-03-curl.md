#### Form input

```bash
curl --location 'http://127.0.0.1:8001/todo' \
    --form 'description="test"' \
    --form 'complete="true"'

curl --location 'http://127.0.0.1:8001/todo' \
    --header 'Content-Type: application/x-www-form-urlencoded' \
    --data-urlencode 'description=test' \
    --data-urlencode 'complete=true'

# or
# Output form errors with:
# 422 Unprocessable Entity
# or
# 415 Unsupported Media Type
```


<aside class="notes">
</aside>
