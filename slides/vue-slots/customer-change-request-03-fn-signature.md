#### Function signature

(breaking change!)

```typescript
// export function removeUndefined<T>(array: T[]): T[] {
export function customFilter<T>(
  array: T[],
  removeUndefined: boolean = true,
  removeNull: boolean = false
): T[] {
  // ...
}
```


<aside class="notes">
</aside>
