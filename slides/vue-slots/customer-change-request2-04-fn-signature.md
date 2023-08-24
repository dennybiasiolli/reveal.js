#### Function signature

```diff
 export function customFilter<T>(
   array: T[],
   removeUndefined: boolean = true,
   removeNull: boolean = false,
   removeEmpty: boolean = false,
+  removeFalse: boolean = false,
+  removeZero: boolean = false,
+  removeZeroString: boolean = false
 ): T[] {
   // ...
 }
```


<aside class="notes">
</aside>
