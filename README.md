# Ruby Bug: Unexpected Behavior with += Operator on Instance Variable

This repository demonstrates an uncommon bug in Ruby related to the unexpected behavior of the += operator when used with instance variables through accessor methods. The bug is caused by the fact that in the provided code, `value=` method returns a copy of the instance variable, leading to the modification not persisting in the instance variable itself. 

## Bug Description
The += operator does not directly modify the instance variable. Instead, it modifies a local copy within the `value=` method, leading to the unexpected output. The solution involves modifying the `value=` method to modify the instance variable directly.