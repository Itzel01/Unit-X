# Lesson-0-Big-O:

## Lesson Overview: 
- 00:00 - 00:05 - What is an Algorithm?
- 00:05 - 00:15 - Algorithm Exploration Activity
- 00:15 - 00:30 - Common Time Complexities
- 00:30 - 00:40 - Quick Touch on Space Complexity
- 00:40 - 01:00 - Why does this matter? (Discussion)


## Objectives: 
- Students should be able to:
  - Determine the time complexity of a problem 
  - Determine the space complexity of a problem 
  - Explain what is time complexity

## Key Terms:
- Big-O Notation
- Runtime Complexity
- Space Complexity
- O(1) - Constant
- O(n) - Linear
- O(n2) - Quadratic
- O(log n) - Log
- O(n * log n) - Log Linear time
- O(2n) - Exponential 
- O(n!) - Factorial

## Key Questions: 
- What is an Algorithm?
- How do we measure the efficiency of an algorithm?
- What are some common time complexities? 
- Why is it important to assess how an algorithm’s runtime grows in relation to the size of its input?

## How this is used: 

Everyone is always saying, time is money and in a company worth millions this is true. Engineers are tasked to always come up with the most efficient algorithms possible! This is because if an application crashes the company will lose a lot of money. 

## Algorithm Analysis:
An algorithm is a set of instructions. Algorithm Analysis is determining the approximate amount of time an algorithm will take based on the operations.  

## Algorithm Activity Solution:

| Append                                                                                                                                                                               | Length of Input | # of Operations |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------|-----------------|
| appendRandom([])                                                                                                                                                                     | 0               | 1               |
| appendRandom(['a'])                                                                                                                                                                  | 1               | 1               |
| appendRandom(['a', 'b'])                                                                                                                                                            | 2               | 1               |
| appendRandom(['a', 'b', 'c', 'd'])                                                                                                                                                  | 4               | 1               |
| appendRandom(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h'])                                                                                                                              | 8               | 1               |
| appendRandom(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p'])                                                                                      | 16              | 1               |
| appendRandom(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'za', 'zb', 'zc', 'zd', 'ze', 'zf']) | 32              | 1               |

| Loop                                                                                                                                                                        | Length of Input | # of Operations |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------|-----------------|
| loop(['a'])                                                                                                                                                                 | 1               | 1               |
| loop(['a', 'b'])                                                                                                                                                            | 2               | 2               |
| loop(['a', 'b', 'c', 'd'])                                                                                                                                                  | 4               | 4               |
| loop(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h'])                                                                                                                              | 8               | 8               |
| loop(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p'])                                                                                      | 16              | 16               |
| loop(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z','za', 'zb', 'zc', 'zd', 'ze', 'zf']) | 32              | 32               |

| Binary Search                                                                                                                                                                              | Length of Input | # of Operations |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------|-----------------|
| binarySearch(['a'], 'a')                                                                                                                                                                  | 1               | 1               |
| binarySearch(['a', 'b'], 'b')                                                                                                                                                             | 2               | 2               |
| binarySearch(['a', 'b', 'c', 'd'], 'c')                                                                                                                                                   | 4               | 2               |
| binarySearch(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h'], 'g')                                                                                                                               | 8               | 3               |
| binarySearch(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p'], 'b')                                                                                       | 16              | 3               |
| binarySearch(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z','za', 'zb', 'zc', 'zd', 'ze', 'zf'], 'zf') | 32              | 6               |


| Nested Loop                           | Length of Input | #  of Operations |
|---------------------------------------|-----------------|------------------|
| nestedLoop(['a'])                     | 1               | 1                |
| nestedLoop(['a', 'b'])                | 2               | 4                |
| nestedLoop(['a', 'b', 'c'])           | 3               | 9                |
| nestedLoop(['a', 'b', 'c', 'd'])      | 4               | 16                |
| nestedLoop(['a', 'b', 'c', 'd', 'e']) | 5               | 25                |


## Common Time Complexities: 

- O(1) - Constant
- O(n) - Linear
- O(n2) - Quadratic
- O(log n) - Log


## What is Space Complexity: 

Another way we can check for efficiency in an algorithm is to see how much memory location we will need to allocate for an algorithm to finish running. For space complexity, we are also looking to see the worst case scenario and we can continue to use Big O to describe the space complexity.  


### Additional Resources: 
- [Intro to Algorithms](https://dev.to/swastikyadav/algorithms-in-javascript-with-visual-examples-gh3)
- [Big O](https://www.freecodecamp.org/news/big-o-notation-why-it-matters-and-why-it-doesnt-1674cfa8a23c/)
- [Resource for this unit!](https://visualgo.net/en)