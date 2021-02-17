# Tuples

## Structure

```cpp
namespace std {
	template <typename... Types> class tuple;
}
```



## Methods

```cpp
#include <tuple>

// Constructors
tuple<T1,T2,...,Tn> t
tuple<T1,T2,...,Tn> t(v1,v2,...,vn)
tuple<T1,T2> t(p) t = t2
t=p
  
// Comparisons
t1 == t2
t1 != t2 
t1 < t2
t1 > t2
t1 <= t2
t1 >= t2 
  
// Operations
t1.swap(t2) 
swap(t1,t2) 
make_tuple(v1,v2,...)
  
tie(ref1,ref2,...) //Creates a tuple of references, which allows extracting (individual) values out of a tuple
```

