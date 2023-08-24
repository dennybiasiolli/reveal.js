#### Implementation

<img src="slides/vue-slots/images/coding.gif" />


<aside class="notes">

```typescript
export function removeUndefined<T>(array: T[]): T[] {
  const retVal: T[] = []
  for (let i = 0; i < array.length; i++) {
    if (array[i] !== undefined) {
      retVal.push(array[i])
    }
  }
  return retVal
}
```

</aside>
