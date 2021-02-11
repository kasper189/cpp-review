# Pairs

## Structure

```cpp
namespace std {
       template <typename T1, typename T2>
       struct pair {
// member
T1 first; T2 second; ...
}; }
```



## Methods

```cpp
//Constructors
pair<T1,T2> p
pair<T1,T2> p(val1,val1)
pair<T1,T2>
pair<T1,T2> p(p2)

// Getters
p.first 
p.second
get<0>(p) get<1>(p) 

// Comparisons
p1 == p2
p1 != p2 p1 < p2
p1 > p2 p1 <= p2 p1 >= p2

// Others
p1.swap(p2) 
swap(p1,p2) 
make_pair(val1,val2)
```

