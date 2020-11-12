# Hash Tables

## Terms:

### **Hash:** 
Is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In a hashtable it is used to determine the index of the array.
It is common for keys to be a 'string' but that is not a requirement.

### **Buckets:** 
Is what is contained in each index of the array of the hashtable. Each index is a bucket and could potentially contain multiple key/value pairs if a collision occurs.

### **Collisions:**
Is what happens when more than one key gets hashed to the same location of the hashtable.

------

**Hashtables** are a data structure that utilizes key value pairs. This means every `NODE` or `BUCKET` has both a key and value.

The basic idea is the ability to store the key into this data structure, and quickly retrieve the value. This is done through a `hash` which is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

Example of hashing in REAL LIFE: In libraries, each book is assigned a unique number that can be used to determine information about the book, such as its exact position in the library or the users it has been issued to etc.

JavaScripts version of a hash table is an object.

An array is a specialization of a hash table.

## HOW TO HASH

If I give it a key I will always get the same value returned

Hashing is implemented in two steps:

1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.
```
hash = hashfunc(key)
index = hash % array_size
```
----

## Resources
[Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

[Video: What is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)

[Basics of Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

[Hash Table Wiki](https://en.wikipedia.org/wiki/Hash_table)