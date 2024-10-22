#### Why Code Quality and Consistency Matter

```py
def double(x):
    return x * 2

numbers = [1, 2, 3, 4]
even_numbers = [num for num in numbers if num % 2 != 0]
doubled_numbers = map(double, even_numbers)
result = sum(doubled_numbers)
print(result)
```
<small>
Why does this code return 8 instead of 12?
</small>


<aside class="notes">
</aside>
