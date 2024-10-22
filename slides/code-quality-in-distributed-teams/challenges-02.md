#### Key Challenges

Tabs vs. spaces, end-of-line style..

```diff
- def get_even_items(all_items):
-     even_items = []
-     for item in all_items:
-         if item % 2 != 0:
-             even_items.append(item)
-     return even_items
+ def get_even_items(all_items):
+     even_items = []
+     for item in all_items:
+         if item % 2 == 0:
+             even_items.append(item)
+     return even_items
```
<small>
What has been changed in this code snippet?
</small>


<aside class="notes">
</aside>
