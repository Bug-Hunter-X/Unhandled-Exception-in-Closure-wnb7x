# Unhandled Exception in Groovy Closure

This example showcases a common error in Groovy: unhandled exceptions within closures. When an exception occurs within a closure passed to a method, if not handled properly, it will propagate up and terminate the program unexpectedly.

The `bug.groovy` file contains the problematic code.  The `bugSolution.groovy` file provides a corrected version with proper exception handling.

## How to Reproduce

1. Save the code in `bug.groovy`.
2. Run the script using a Groovy interpreter (e.g., `groovy bug.groovy`).
3. Observe that the program terminates before printing "This line will not be reached".

## Solution

The solution involves using a `try-catch` block within the method calling the closure to handle potential exceptions.