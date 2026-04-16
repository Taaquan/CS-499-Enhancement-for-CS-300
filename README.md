# CS-499-Enhancement-for-CS-300

# Course Data Management System Enhancement

## Overview

This artifact is based on a project developed in CS 300: Data Structures and Algorithms. The application is designed to load, store, and display course information from a CSV file, including course numbers, titles, and prerequisites.

The enhanced version of this project focuses on improving efficiency, data validation, and overall program structure using appropriate data structures and algorithmic techniques.

---

## Enhancement Summary

The project was enhanced to improve reliability, performance, and usability. Key improvements include:

* Stronger input validation when loading CSV data
* Validation of prerequisite relationships between courses
* Improved search functionality with consistent formatting
* Increased efficiency by removing unnecessary sorting operations
* Prevention of duplicate data when reloading the dataset
* Improved modular design through helper functions

---

## Technical Improvements

### Data Structure Optimization

The program uses a map to store course data, which automatically maintains sorted order. This allowed the removal of unnecessary sorting operations, improving efficiency and simplifying the code.

### Algorithm Efficiency

* Original approach: Sorting course data using a vector (O(n log n))
* Improved approach: Direct traversal of map (O(n))
* Search improvement: Map-based lookup (O(log n)) instead of linear search (O(n))

### Validation Enhancements

* Trimmed whitespace from all input fields
* Converted course IDs and prerequisites to uppercase
* Skipped invalid or incomplete rows
* Checked for duplicate course entries
* Verified that prerequisites exist in the dataset

### Modular Design

Helper functions were added to improve code organization and readability, including:

* `trim()` for cleaning input data
* `validatePrerequisites()` for ensuring data integrity

---

## Testing

The application was tested using multiple scenarios to ensure correct functionality:

* Loading valid and invalid CSV data
* Verifying duplicate prevention
* Testing prerequisite validation warnings
* Searching for courses with different input formats
* Printing the course list to confirm sorted output

The enhanced version showed improved performance by eliminating unnecessary sorting and using efficient search operations.

---

## Skills Demonstrated

This artifact demonstrates the following computer science skills:

* Algorithm design and optimization
* Time complexity analysis (Big-O notation)
* Data structure selection and implementation
* Input validation and error handling
* Modular programming and code organization
* Performance improvement through efficient design

---

## Outcome Alignment

This enhancement aligns with key Computer Science program outcomes:

* Designing and evaluating efficient computing solutions
* Applying data structures and algorithms to real-world problems
* Improving performance through algorithm optimization
* Developing maintainable and scalable software systems

---

## Reflection

Through this enhancement, I learned how important it is to select the correct data structure for a problem. Using a map instead of manually sorting data improved both performance and code simplicity. I also gained experience in analyzing algorithm complexity and understanding how small changes can significantly impact efficiency.

This project helped strengthen my ability to think critically about performance, scalability, and data organization, which are essential skills in software development.
