#### Implementation

```typescript
export function customFilter<T>(
  array: T[],
  filterFn: (element: T, index: number, array: T[]) => boolean
): T[] {
  const retVal: T[] = []
  for (let i = 0; i < array.length; i++) {
    if (filterFn(array[i], i, array)) {
      retVal.push(array[i])
    }
  }
  return retVal
}
```

<aside class="notes">
</aside>
