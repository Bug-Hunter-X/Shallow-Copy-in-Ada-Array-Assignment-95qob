# Ada Shallow Copy Pitfall

This repository demonstrates a common pitfall in Ada programming involving array assignments.  In Ada, when you assign one array to another, it performs a shallow copy, not a deep copy.  This means both variables point to the same underlying data. Changes to one array's elements affect the other.

The `bug.ada` file shows an example of this behavior, while `bugSolution.ada` provides the corrected code using an explicit loop for deep copying.

**Key takeaway:** Always be mindful of shallow vs. deep copies when working with composite data types in Ada, especially when modifying arrays after assignment.