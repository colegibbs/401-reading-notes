# Reading: hash-tables

## Hash Table Cheat Sheet

- hash is being used to determine the index of an array
- a bucket is what is contained at each index of the array
- a collision is when more than one key gets assigned to a bucket
- why:
  - hold values
  - dictionary
  - library
- every node has a key and value
- hash allows you to go diretly to the location of the key
- hash searching is O(1) time complexity
- place useing hash functions that put each item at an index based off it's key
- same key should always produce same hash code
- can use ASCII values to create the hash code
- if two buckets have the same index that needs to be handled
- if to values are stored at the same index then use a linked list at that index 
- hash table can recognize load factor and grow if needed
- methods: add(), find(), contains(), getHash()