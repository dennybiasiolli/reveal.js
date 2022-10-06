#### Axios interceptors

```js
axios.defaults.baseURL = `http://localhost:3000/api`;
// axios.get('/orders')
```

```js
axios.interceptors.request.use(
  async (request) => request,
  // request.headers.Authorization = `Bearer ${token}`;

  async (error) => { throw error }
)
```

```js
axios.interceptors.response.use(
  async (response) => response,

  async (error) => {
    // if (!err.response) { /* Server connection lost */ }
    // if (err.response.status === 401) { /* Unauthorized */ }
    throw error
  }
)
```


<aside class="notes">

https://axios-http.com/docs/interceptors

</aside>
