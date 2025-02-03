# Elixir Enum.each List Modification Issue

This repository demonstrates an unexpected behavior when attempting to modify a list while iterating over it using `Enum.each` in Elixir.  The provided code snippet attempts to remove an element from the list during iteration, which does not modify the original list as one might expect.

## Problem Description

The code iterates through a list and attempts to delete an element if a condition is met.  However, because `Enum.each` does not modify the original list, the deletion operation doesn't impact the iteration. The `IO.inspect` shows that the original list is unmodified.

## Solution

The solution involves using a different approach that appropriately modifies the list, such as using `Enum.filter` or list comprehension.
