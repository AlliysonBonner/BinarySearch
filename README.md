# Binary Search Algorithm

This is an implementation of the Binary Search Algorithm in Python. The algorithm uses the divide and conquer approach to search for an element in a sorted list.

There are two algorithms implemented:
* Naive Search Algorithm
* Binary Search Algorithm

## Naive Search Algorithm

The Naive Search Algorithm scans the entire list and compares each element with the target element. If the element is found, it returns the index of the element in the list, else it returns -1.

## Binary Search Algorithm

The Binary Search Algorithm uses the divide and conquer approach to search for the target element in a sorted list. The algorithm first checks the middle element of the list. If the middle element is equal to the target, it returns the index of the middle element. If the target is less than the middle element, the algorithm searches in the left half of the list. If the target is greater than the middle element, the algorithm searches in the right half of the list. The algorithm continues to search in the half of the list where the target may exist. If the target is not found, the algorithm returns -1.

## Usage

To use the algorithm, you can call the functions with the required parameters.

```python
from binary_search import naive_search, binary_search

l = [1, 3, 5, 10, 12]
target = 7

naive_search_result = naive_search(l, target)
binary_search_result = binary_search(l, target)

print("Naive search result:", naive_search_result)
print("Binary search result:", binary_search_result)

## Performance
To test the performance of the algorithms, a sorted list of 10000 random elements is generated. Both algorithms are called to search for each element in the list. The average time taken by each algorithm is calculated and printed.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
