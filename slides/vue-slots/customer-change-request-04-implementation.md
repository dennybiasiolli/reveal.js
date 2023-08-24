#### Implementation

<img src="slides/vue-slots/images/cats-coding.gif" />


<aside class="notes">

```typescript
export function customFilter<T>(
  array: T[],
  removeUndefined: boolean = true,
  removeNull: boolean = false
): T[] {
  const retVal: T[] = []
  for (let i = 0; i < array.length; i++) {
    if (
      (removeUndefined && array[i] === undefined) ||
      (removeNull && array[i] === null)
    ) {
      continue
    }
    retVal.push(array[i])
  }
  return retVal
}
```

</aside>
