# Vector Implementation in C++

This project is a C++ implementation of a dynamic array class called `Vector`. The `Vector` class mimics the behavior of the standard `std::vector` in C++, providing a custom implementation with various methods to manage and manipulate the elements stored in the dynamic array.

## Features

### Core Functionality
- **Dynamic Memory Management:** 
  - Automatically resizes when the capacity is exceeded.
  - Initial capacity is set to 10 elements.
  
- **Element Access:**
  - `at(int index)`: Accesses the element at the given index.
  - `front()`: Returns a reference to the first element.
  - `back()`: Returns a reference to the last element.
  
- **Modifiers:**
  - `push_back(int value)`: Adds an element to the end of the vector.
  - `pop_back()`: Removes the last element from the vector.
  - `insert(int index, int value)`: Inserts an element at the specified index.
  - `erase(int index)`: Removes the element at the specified index.
  - `swap(Vector &other)`: Swaps the contents of the vector with another vector.
  - `clear()`: Removes all elements from the vector.

- **Capacity and Size:**
  - `getSize()`: Returns the current number of elements in the vector.
  - `getCapacity()`: Returns the current capacity of the vector.
  - `empty()`: Checks if the vector is empty.

- **Utility Functions:**
  - `begin()`: Returns a pointer to the first element.
  - `end()`: Returns a pointer to the past-the-end element.
  - `display()`: Prints all the elements in the vector.

### Testing
- The `main()` function demonstrates and tests the functionality of the `Vector` class by:
  - Adding elements to the vector using `push_back()`.
  - Displaying the elements.
  - Swapping two vectors.
  - Checking the size and capacity.
  - Removing the last element using `pop_back()`.
  - Accessing and displaying the front and back elements.
  - Inserting an element at a specific index.
  - Erasing an element from a specific index.
  - Displaying elements using the `begin()` and `end()` pointers.
  - Clearing the vector and checking if it is empty.

## How to Use

1. **Compilation:** Compile the program using a C++ compiler:
   ```bash
   g++ -o vector_example vector.cpp
   ```

2. **Execution:** Run the compiled program:
   ```bash
   ./vector_example
   ```

3. **Expected Output:** The program will test various methods of the `Vector` class and output the results, demonstrating the correct functionality of each method.

## Example Usage
```cpp
Vector v1;
v1.push_back(10);
v1.push_back(20);
v1.insert(1, 15);  // Inserts 15 at index 1
v1.display();      // Outputs: 10, 15, 20
v1.pop_back();     // Removes the last element (20)
v1.display();      // Outputs: 10, 15
```

## Conclusion
This project provides a simple and efficient implementation of a dynamic array in C++, showcasing the fundamental operations that can be performed on a vector. The `main()` function serves as a comprehensive test bed to ensure that all operations work as expected.
