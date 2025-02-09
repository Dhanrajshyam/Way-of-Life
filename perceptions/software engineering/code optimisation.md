# **Code Optimization Objectives**

Wisdom talk: Find the most useful information(minimum required information) quickly to solve the given problem quickly using best strategy known today. Then find new ways. **You dont know everything.**

## **Time Optimization**
- **Improve Processing Time**  
  - Reduce the time taken to produce the output for a given input.
  - Optimize algorithms to reduce time complexity (e.g., `O(n²) → O(n log n)`).
  - Utilize vectorized operations (e.g., NumPy, Pandas) instead of loops.

- **Improve Data Transport Time**  
  - Minimize the time taken to retrieve and send data between **storage ↔ memory (RAM/CPU cache) ↔ processor**.
  - Use **efficient data storage formats** (e.g., Parquet, Protobuf) to reduce I/O time.
  - Apply **data locality principles** to minimize cache misses.

- **Improve Function Retrieving Time**  
  - Reduce the time taken to fetch functions from memory (RAM/CPU cache) to the processor.
  - Utilize **function inlining** and **JIT (Just-In-Time) compilation** where applicable.
  - Preload frequently used functions to avoid repetitive memory fetches.

- **Improve Data Sanitizing Time**  
  - Minimize the time taken to remove unnecessary data and retain only useful information in an organized way.
  - Use **efficient filtering techniques** (e.g., list comprehensions instead of loops).
  - Optimize **string manipulations** (e.g., regex vs. direct string operations).

- **Parallelism & Concurrency Optimization**  
  - Use **multithreading, multiprocessing**, or **async processing** to speed up execution.
  - Leverage **batch processing** instead of processing elements one by one.

- **Cache Optimization**  
  - Use **memoization** and **caching techniques** to reduce redundant computations.
  - Optimize **memory access patterns** to avoid CPU cache misses.

---

## **Memory Optimization**
- **Keep Only Cleaned Data in Memory**  
  - Store only essential data in active memory and remove unnecessary variables.
  - Optimize Python's **Garbage Collection (GC)** (e.g., `gc.collect()` when necessary).

- **Organize Data for Quick Accessibility**  
  - Structure data to be quickly accessible by processing units.
  - Use **indexed data structures** (e.g., hash maps, B-trees) for faster lookups.

- **Compression & Data Deduplication**  
  - Use **efficient encoding** (e.g., gzip, protobuf) to reduce memory usage.
  - Remove **duplicate data** before storing it in memory.

- **Streaming & Lazy Loading**  
  - Process large datasets using **streaming techniques** instead of loading them fully into memory.
  - Use **lazy evaluation** (e.g., Python generators, iterators) to avoid excessive memory allocation.

---

