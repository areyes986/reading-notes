## Hashtables

They are data structures that utilize key/value pairs. Each node or bucket has a key and a value. Hashtables store keys into a data structure and retrieve the value which is done through a hash. It encodes the key and it will map to a specific location in the structure so we can retrieve the value. For time is will be O(1) because we use the hash to the key to find the exact location of the value.  

**Hash:** Usually used for security, a hash is the result of an algorithm taking a string to turn it into a value. A *hashtable* its used to find the index of an array. Hashing is used to identify a specific object from a group of similar objects. A hash function is used to map a data set of a random size of data to a data set that is fixed. Thats that are returned are called hask values, hash codes, hash sums or just hashes.  
*Creating a Hash*  
It is created from an array and after it is created to the appropriate size, turn the key into a numerical value. We can:  
1. Add/multipy ASCII values
2. Multiply by a prime #
3. Use modulo to get the remainder of the result, then divide by the size of the array
4. Insert into the array at the index.   

**Buckets:** contained in the index of the array of the hashtable. An index is a bucket and can have more than one key/value pair if collision occurs.  If a hash map has few buckets is can have more collisions because it is densely full.
**Collision:** when more than one key gets hashed to the same location on the hashtable.  To solve this, you would call the method `.Add(key, value)` with different keys to overwrite each other. 

**Internal Methods**  
1. Add() - adds a new key/value pair to a hashtable, key gets the GetHash method, finds the index, goes to it, checks if something exists in the index already, if not, add the key/value pair, if it does, add the pair to the data structure within the bucket. 
2. Find() - takes the keys, gets the hash then goes to the indexes location. 
3. Contains() - accept the key, returns a bool if the key exists inside the hashtable. 
4. GetHash() - accept the key as a string, do that hash, then returns the index.






