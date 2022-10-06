#### WebSocket

<small>

https://developer.mozilla.org/en-US/docs/Web/API/WebSocket

</small>

```js
let socket = null

onMounted(() => {
  // Create WebSocket connection.
  socket = new WebSocket('ws://localhost:8080')
```

```js
  // Connection opened
  socket.addEventListener('open', (event) => {
    socket.send('Hello Server!')
  })
  
  // Listen for messages
  socket.addEventListener('message', (event) => {
    console.log('Message from server ', event.data)
  })
})
```


<aside class="notes">

https://developer.mozilla.org/en-US/docs/Web/API/WebSocket

https://pusher.com/

</aside>
