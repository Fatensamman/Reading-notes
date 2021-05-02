# Hash Tables

[Link to CF article](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

## What is a Hashtable?

1. Hashtable is a data structure used to store information. 

1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

1. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

1. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

## Use:

- Hold unique values
- Dictionary
- Library

## More about Hashtable
- ability to store the key into this data structure, and quickly retrieve the value. 

- A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

- we can do a lookup in an O(1) time complexity

## Structure

- hash code turns a key into an integer. 
- The same key should always produce the same hash code.
- should never have randomness to them.

## Collisions

- occurs when more than one key hashes to the same index in an array
- “perfect hash” will never have any collisions.
- Collisions are solved by changing the initial state of the buckets. Instead of starting them all as null we can initialize a LinkedList in each one.
- Each index in the array is called a “bucket” because it can store multiple key/value pairs.
- different keys can lead to the same bucket it’s important to store the entire key/value pair in the bucket, not just the value. 

### Hash maps do this to store values:

- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- store the key with the value by appending both to the end of a linked list

### Hash maps do this to read value:

- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- use the array index to access the short LinkedList representing a bucket
- search through the bucket looking for a node with a key/value pair that matches the key you were given

## Internal Methods
### Add()
When adding a new key/value pair to a hashtable:

- send the key to the GetHash method.
- Once you determine the index of where it should be placed, go to that index
- Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
- If something does exist, add the new key/value pair to the data structure within that bucket.

### Find()
The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

### Contains()
The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the key exists in the table given the index returned.

### GetHash()
The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.

[The basics of Hash Table](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)