#### Render Scope

Slot content

- has access to the data scope of the parent component

    ```html
    <span>{{ message }}</span>
    <FancyButton>{{ message }}</FancyButton>
    ```

- does <u>not</u> have access to the child component's data


<aside class="notes">
</aside>
