Bad code travels fast in distributed teams.

```text
def p(x):return x*2
l=[1,2,3,4]
x=[i for i in l if i%2!=0]
y=map(lambda x:p(x),x)
z=sum(y)
print(z)
```

<small>If your code looks like this, it's time for a refactor!</small>
