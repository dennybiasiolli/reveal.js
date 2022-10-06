#### Axios usage

```bash
npm install --save axios
```

```js
import axios from 'axios'
```

```js
axios.get('/products')
  .then((response) => {
    console.log(response)
  })
  .catch((error) => {
    console.error(error)
  })
```

```js
try {
  const response = await axios.get('/products')
  console.log(response)
} catch (error) {
  console.error(error)
}
```


<aside class="notes">

https://axios-http.com/docs/example

</aside>
