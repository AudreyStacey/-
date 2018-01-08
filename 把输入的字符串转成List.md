

```python
x=input('以逗号隔开')
xlist=x.split(",")
xlist = [int(xlist[i]) for i in range(len(xlist))] 
print(xlist)
```

    以逗号隔开1,2,3,4
    [1, 2, 3, 4]
    
