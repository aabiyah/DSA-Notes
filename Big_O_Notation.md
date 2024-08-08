# Complexity Comparison Between Typical Big Os

## O(1) - Constant Time Complexity

**Description:** Algorithms with constant time complexity execute in a constant amount of time regardless of the input size.

**Example:** Accessing an element in an array by index.

**Comparison:** Regardless of the input size, the time is the same.

## O(log n) - Logarithmic Time Complexity

**Description:** Algorithms with logarithmic time complexity have their runtime grow logarithmically with the input size.

**Example:** Binary search in a sorted array.

**Comparison:** As the input size increases, the runtime grows slowly, making it more efficient than linear time complexities.

## O(n) - Linear Time Complexity

**Description:** Algorithms with linear time complexity have their runtime grow linearly with the input size.

**Example:** Linear search through an unsorted array.

**Comparison:** The runtime increases proportionally to the input size.

## O(n log n) - Linearithmic Time Complexity

**Description:** Algorithms with linearithmic time complexity have their runtime grow in proportion to the input size multiplied by the logarithm of the input size.

**Example:** Efficient sorting algorithms like mergesort and heapsort.

**Comparison:** More efficient than quadratic time complexities but less efficient than linear or logarithmic ones.

## O(n^2) - Quadratic Time Complexity

**Description:** Algorithms with quadratic time complexity have their runtime grow quadratically with the input size.

**Example:** Nested loops iterating over the input.

**Comparison:** As the input size increases, the runtime grows quadratically, making it less efficient for large inputs.

## O(2^n) - Exponential Time Complexity

**Description:** Algorithms with exponential time complexity have their runtime grow exponentially with the input size.

**Example:** Brute-force algorithms that try all possible combinations.

**Comparison:** Extremely inefficient for large inputs, as the runtime increases rapidly with even small increases in input size.

## O(n!) - Factorial Time Complexity

**Description:** Algorithms with factorial time complexity have their runtime grow factorially with the input size.

**Example:** Algorithms generating all permutations of a set.

**Comparison:** Highly inefficient, with the runtime growing extremely fast with the input size.

# Time & Space Complexity

## Time Complexity

Time complexity refers to an algorithm's time to complete its execution as a function of the input size. It helps understand how an algorithm's runtime scales with different input sizes. Time complexity is typically expressed using Big O notation to describe the upper bound of the algorithm's runtime.

For example:

- **O(1)** represents constant time complexity, indicating that the algorithm's runtime does not change with the input size.
- **O(log n)** represents logarithmic time complexity, where the runtime grows logarithmically as the input size increases.
- **O(n)** represents linear time complexity, where the runtime grows linearly with the input size.
- **O(n^2)** represents quadratic time complexity, where the runtime grows quadratically with the input size.
- **O(2^n)** represents exponential time complexity, where the runtime grows exponentially with the input size.

Analyzing time complexity helps in understanding the efficiency of algorithms, comparing different algorithms for the same problem, and predicting their performance under varying input sizes.

## Space Complexity

Space complexity refers to the amount of memory an algorithm uses to execute as a function of the input size. It helps understand how much memory an algorithm requires to store data and execute operations. Similar to time complexity, space complexity is also expressed using Big O notation to describe the upper bound of the algorithm's memory usage.

For example:

- **O(1)** represents constant space complexity, indicating that the algorithm uses a fixed amount of memory regardless of the input size.
- **O(n)** represents linear space complexity, where the memory usage grows linearly with the input size.
- **O(n^2)** represents quadratic space complexity, where the memory usage grows quadratically with the input size.

Analyzing space complexity is essential for understanding the memory requirements of algorithms, optimizing memory usage, and ensuring efficient resource utilization, especially in memory-constrained environments.

# Complexity: Best, Average, Worst, Expected

| Complexity | Best Case | Average Case | Worst Case | Expected Case |
|------------|-----------|--------------|------------|---------------|
| **O(1)**   | O(1)      | O(1)         | O(1)       | O(1)          |
| **O(log n)** | O(1)    | O(log n)     | O(log n)   | O(log n)      |
| **O(n)**   | O(n)      | O(n)         | O(n)       | O(n)          |
| **O(n log n)** | -     | O(n log n)   | O(n log n) | O(n log n)    |
| **O(n^2)** | -         | O(n^2)       | O(n^2)     | O(n^2)        |
| **O(2^n)** | -         | -            | O(2^n)     | O(2^n)        |
| **O(n!)**  | -         | -            | O(n!)      | O(n!)         |

## Explanation

### Best Case

Represents the minimum time or space required by the algorithm for any input. It's often an optimistic scenario.

### Average Case

Represents the expected time or space required by the algorithm averaged over all possible inputs. It provides a more realistic estimation of performance.

### Worst Case

Represents the maximum time or space required by the algorithm for any input. It's often a pessimistic scenario.

### Expected Case

Represents the average time or space complexity under some probabilistic model, providing insight into performance with more nuanced assumptions than simple average-case analysis.


