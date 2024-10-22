#### Key Challenges

CamelCase vs. snake_case..

```diff
- def getEvenItems(allItems):
-     evenItems = []
-     for item in allItems:
-         if item % 2 != 0:
-           evenItems.append(item)
-     return evenItems
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
