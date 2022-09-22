#### Test migration

- mutations: &rarr; actions

- actions

    use `.call` to pass state/getters/actions

    ```diff
    -const context = { commit: vi.fn() }
    -actions.incrementAsync(context)
    +const state = { increment: vi.fn() }
    +actions.incrementAsync.call(state)
        // ...
    -expect(context.commit).toHaveBeenCalled()
    +expect(state.increment).toHaveBeenCalled()
    ```


<aside class="notes">
</aside>
