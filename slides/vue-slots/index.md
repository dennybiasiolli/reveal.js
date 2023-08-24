![Vue logo](slides/vue-slots/images/vue-logo.svg)

### Vue.js slots

<!-- Don't get swamped with customization requests! -->
Non farti sommergere dalle richieste di personalizzazione!

&nbsp;

<small>

#### Commit University

Firenze, 19 Ottobre 2023

</small>


<aside class="notes">
Sometimes being lazy is a quality, avoid (almost) any customization requests by leaving "open windows" in your generic components.

Slots are a way to pass content to a component in Vue.js. They allow you to define a section of a component’s template that can be replaced by the parent component.

Slots can also be named or scoped, which provide more control and customization over the slot content. Named slots allow you to define multiple slots in a component and target them with specific names. Scoped slots allow you to access the child component's data in the slot content.

Let's analyze some real-world examples on using slots, including

- Slot Content and Outlet
- Render Scope
- Fallback Content
- Named Slots
- Scoped Slots
- ...pizza! :)
- testing
</aside>
