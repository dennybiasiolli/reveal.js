#### Why Code Quality and Consistency Matter

```py
def p(x):return x*2
def s(l):return sum(l)
l=[1,2,3,4]
x=[i for i in l if i%2!=0]
y=map(lambda x:p(x),x)
z=s(y)
print(z)
```
<small>
Why does this code return 8 instead of 12?
</small>


<aside class="notes">
</aside>
