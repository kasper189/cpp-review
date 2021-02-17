# Arrays

## Structure

```cpp
namespace std {
	template <typename T, size_t N> class array;
}
```



## Methods

```cpp
#include <array>

std::array<int,4> x = {};
std::array<int,5> coll = { 42, 377, 611, 21, 44 };

// Swap
std::array<std::string,10> as1, as2;
as1 = std::move(as2);

// Constructors
array<Elem,N> c 
array<Elem,N> c(c2) 
array<Elem,N> c = c2
  
// Operations
c.empty()
c.size() 
c.max_size() // Returns the maximum number of elements possible
// size and max_size of an array object always match
c = c2
c = rv 
c.fill(val) 
c1.swap(c2) 
swap(c1,c2)

// Comparisons
c1 == c2
c1 != c2
c1 < c2
c1 > c2
c1 <= c2
c1 >= c2
 
// Access
c[idx] 
c.at(idx) // it's the only one to perform range-checking => throws an out_of_range exception
c.front() 
c.back()
  
// Iterators
c.begin() 
c.end() 
c.cbegin() 
c.cend()
c.rbegin() // Returns a reverse iterator for the first element of a reverse iteration
c.rend()
c.crbegin() 
c.crend()
```



## Tuple interface

```cpp
typedef std::array<std::string,5> FiveStrings; 

FiveStrings a = { "hello", "nico", "how", "are", "you" };

std::tuple_size<FiveStrings>::value // yields 5
std::tuple_element<1,FiveStrings>::type // yields std::string
std::get<1>(a) // yields std::string("nico")
```

