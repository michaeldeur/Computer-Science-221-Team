# Team Byte Me - Lists Project

## Overview

This project implements and tests various list data structures in Java, focusing on arraylists and linked lists. The codebase includes custom implementations, comprehensive unit tests, and scenario-based testing for correctness and robustness, including iterator and list iterator behaviors.

## Team

**Team Name:** Team Byte Me

## Project Structure

```
.gitattributes
BadList.java
BidirectionalNode.java
GoodList.java
IndexedUnsortedList.java
IteratorTestScenarios.txt
IUArrayList.java
IUDLLReferenceCode.java
IUDoubleLinkedList.java
IUSingleLinkedList.java
Lab07_Lists_Pt1.pdf
Lab08_Lists_Pt2.pdf
Lab09_ArrayList.pdf
Lab10_SLL.pdf
Lab11_DLL.pdf
LinearNode.java
ListIteratorTests.txt
ListTester.java
ListTests.txt
README.md
```

## Key Files

- **BidirectionalNode.java**  
  Implements a doubly-linked node for use in linked list structures.  
  Provided as a reference for node operations.

- **IndexedUnsortedList.java**  
  Interface for an indexed, unsorted list with methods for adding, removing, and accessing elements.

- **IUDoubleLinkedList.java**  
  Your main implementation of a doubly-linked list that supports indexed and unsorted operations.

- **IUArrayList.java**  
  Array-based implementation of the indexed unsorted list.

- **IUSingleLinkedList.java**  
  Singly-linked list implementation.

- **ListTester.java**  
  Comprehensive test suite for all list implementations, including iterator and list iterator scenarios.  
  Provided in part; you will complete and use this for validation.

- **ListIteratorTests.txt, ListTests.txt, IteratorTestScenarios.txt**  
  Text files describing required and optional test scenarios for iterators and list iterators.

- **Lab07_Lists_Pt1.pdf, Lab08_Lists_Pt2.pdf, Lab09_ArrayList.pdf, Lab10_SLL.pdf, Lab11_DLL.pdf**  
  Assignment instructions and specifications.  
  **Read these for detailed requirements and grading rubrics.**

## How to Build and Run

1. **Compile All Java Files**

   ```sh
   javac *.java
   ```

2. **Run the Test Suite**

   ```sh
   java ListTester
   ```

   - By default, only failed tests are printed.
   - Use command-line flags for more output:
     - `-a` : Print all test results (not just failures)
     - `-s` : Hide string outputs from `toString()` tests
     - `-m` : Hide section summaries

   Example:

   ```sh
   java ListTester -a
   ```

## Implementation Notes

- **BidirectionalNode**  
  Used for doubly-linked list implementations.  
  Provides `getNext()`, `setNext()`, `getPrevious()`, `setPrevious()`, `getElement()`, and `setElement()` methods.

- **IndexedUnsortedList**  
  Defines the required API for all list implementations, including indexed access, addition, removal, and search.

- **Iterators and ListIterators**  
  Your implementations must provide correct fail-fast behavior, support for concurrent modification detection, and all required iterator/list iterator methods as described in the PDF instructions and test files.

- **Testing**  
  The provided [`ListTester.java`](ListTester.java) runs a wide range of scenarios, including:
  - Basic list operations
  - Iterator and ListIterator correctness
  - Edge cases (empty lists, out-of-bounds, etc.)
  - Concurrency and fail-fast behavior

  Review [`ListIteratorTests.txt`](ListIteratorTests.txt) and [`ListTests.txt`](ListTests.txt) for the full list of required behaviors.

## Assignment Requirements

- **Follow the specifications in the PDF files**  
  - [Lab07_Lists_Pt1.pdf](Lab07_Lists_Pt1.pdf)
  - [Lab08_Lists_Pt2.pdf](Lab08_Lists_Pt2.pdf)
  - [Lab09_ArrayList.pdf](Lab09_ArrayList.pdf)
  - [Lab10_SLL.pdf](Lab10_SLL.pdf)
  - [Lab11_DLL.pdf](Lab11_DLL.pdf)

- **Implement all required methods and behaviors**
- **Pass all provided and described tests**
- **Document your code where appropriate**

## Tips

- Start by understanding the provided [`BidirectionalNode.java`](BidirectionalNode.java) and [`ListTester.java`](ListTester.java).
- Implement and test incrementally.
- Use the test output to guide debugging and ensure full coverage.
- Consult the PDFs for clarifications on method behaviors and edge cases.

## Credits

- Portions of several files including parts of [`ListTester.java`](ListTester.java) was provided by course staff.
- All other code and documentation by **Team Byte Me**.

---
