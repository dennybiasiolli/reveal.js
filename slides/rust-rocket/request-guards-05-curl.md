#### Request Guard examples

```bash
curl --location 'http://127.0.0.1:8000/api/sensitive'
# Output: 400 Bad Request

curl --location 'http://127.0.0.1:8000/api/sensitive' \
    --header 'x-api-key: valid_api_key'
# Output: Sensitive data.
```


<aside class="notes">
</aside>
