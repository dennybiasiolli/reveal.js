#### Test migration

- state: no changes

- getters

    use `.call` on a getter when using `this` to access other getters

    ```diff
    -expect(getters.isOdd({}, { isEven: false })).toBe(true)
    +expect(getters.isOdd.call({ isEven: false })).toBe(true)
    ```


<aside class="notes">
</aside>
