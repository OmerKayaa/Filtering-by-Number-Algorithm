# Filtering by Number Algorithm

#### Filtering by Number Algorithm is a data structure algorithm aims to increase performance of set operations like
- Find Union
- Find Disjuction
- Find Intersection
- Find Subtraction

## Project Summary

Every real number is either a prime number or multiplication of prime numbers. Finding if a number is multiple of a prime number is a easy task for a computer. You can simply find out using mod(modulus) operator. If number mod prime is 0 it means number is multiple of that prime number and you can easily make number not multiple of that prime by simply dividing it to that prime number and again if you want to make a number mulptiple of a prime number you can easily do it by multiplying to that prime number. The point is you can think every number as a bag of prime numbers. 

### Example

105 is 7 * 5 * 3 so 105 multiplication of three prime numbers and let say we want to subtract one of the primes like 3 we can do it by simply dividing 105 to 3 which is 35 and 35 is 7 * 5

What if we use this property to make a data structure like a list?
All we need to do is a table to know which prime number represent which object.
This project is a proof that using prime numbers to build a data structure is possible and efficient.

## Performace (in Theory)

To increase performance I used Euclidean Greatest common divisor algorithm (GCD) it alowed me to find common primes numbers at time complexity of Log N

Command / Algorithm | Linked List | Array List | FNA
--- | --- | --- | ---
 `get()` | **O(N)** | **O(1)** | **O(1)** 
 `add()` | **O(1)** | **O(1)** | **O(1)** 
 `remove()` | **O(1)** | **O(N)** | **O(Log(N))** 
 `find()` | **O(N)** | **O(N)** | **O(Log(N))** 
 `contains()` | **O(N)** | **O(N)** | **O(Log(N))** 
 
 Table below is the comparison how well x algorithm doing when it used on itself.
 
 example: Arraylist.addAll(ArrayList)
 
 Algorithm / Algorithm | Linked List | Array List | FNA
--- | --- | --- | ---
 `addAll()` | **O(N)** | **O(N)** | **O(1)** 
 `removeAll()` | **O(N)** | **O(N^2)** | **O(Log(N))** 
 `retailAll()` | **O(N^2)** | **O(N^2)** | **O(Log(N))** 
 `containsAll()` | **O(N^2)** | **O(N^2)** | **O(Log(N))** 
 
 ### Graphs
 
 Command | Performance
--- | ---
`get()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Command/get.png" width="30%"> 
`add()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Command/add.png" width="30%">
`remove()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Command/remove.png" width="30%">
`find()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Command/contain-search.png" width="30%">
`contains()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Command/contain-search.png" width="30%">

---

Algorithm | Performance
--- | ---
`addAll()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Algoritm/AddAll.png" width="30%">
`removeAll()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Algoritm/RemoveAll.png" width="30%">
`retailAll()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Algoritm/RetailAll-ContainsAll.png" width="30%">
`containsAll()` | <img src="https://github.com/OmerKayaa/Filtering-by-Number-Algorithm/blob/master/Presention(non-essential)/Algoritm/RetailAll-ContainsAll.png" width="30%">

