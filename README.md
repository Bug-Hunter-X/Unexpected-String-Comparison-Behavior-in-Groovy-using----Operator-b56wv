# Groovy String Comparison Bug

This repository demonstrates a common error in Groovy related to comparing strings using the `==` operator.  The `==` operator in Groovy performs reference equality checks, not value equality checks for strings. This can lead to unexpected results when working with `null` or empty strings.

## The Bug
The provided `bug.groovy` file contains a method `myMethod` that attempts to handle `null` and empty strings. However, it uses `==` for comparison, which results in incorrect behavior.  The example showcases how the outputs are not as expected due to the use of `==`.

## The Solution
The `bugSolution.groovy` file demonstrates the corrected version, which uses the `.equals()` method for proper string comparison.  This ensures that values are compared correctly, regardless of whether the strings are null or empty.

## How to Run
1. Clone the repository.
2. Ensure you have Groovy installed.
3. Navigate to the repository directory using the command line.
4. Run the Groovy scripts:
   ```bash
groovy bug.groovy
groovy bugSolution.groovy
```
Observe the differences in output between the two files.