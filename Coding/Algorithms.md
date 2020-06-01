Newtons method to find square root 
```
long r = x;  
while (r*r > x)
r = (r + x/r) / 2;
return (int) r;
```
    
Also a binary search will also be useful for finding the square root by setting x as upper and 0 as lower.     
