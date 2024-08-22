# Assignment-task

### **Problem: Implement a LRU (Least Recently Used) Cache**

**Description:**

You are required to implement a class `LRUCache` that simulates a cache with a Least Recently Used (LRU) eviction policy. The cache should have the following methods:

1. `__init__(self, capacity: int)`: Initializes the cache with a fixed capacity.
2. `get(self, key: int) -> int`: Returns the value associated with the key if it exists in the cache; otherwise, returns `-1`.
3. `put(self, key: int, value: int) -> None`: Inserts or updates the value for the key. If the cache exceeds its capacity, it should evict the least recently used item.

**Constraints:**

- The operations `get` and `put` should both run in O(1) time.
- Assume the keys and values are integers.
- The cache should store up to `capacity` items. When it reaches this limit, it should evict the least recently used item before inserting a new one.

**Example:**

```python
cache = LRUCache(2)

cache.put(1, 1)
cache.put(2, 2)
print(cache.get(1))       # returns 1
cache.put(3, 3)           # evicts key 2
print(cache.get(2))       # returns -1 (not found)
cache.put(4, 4)           # evicts key 1
print(cache.get(1))       # returns -1 (not found)
print(cache.get(3))       # returns 3
print(cache.get(4))       # returns 4
```
