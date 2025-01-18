# PHP Foreach Loop and unset() on Associative Arrays

This repository demonstrates an uncommon bug in PHP related to the use of `unset()` within a `foreach` loop when iterating over associative arrays.

The issue arises because modifying the array (using `unset()`) while iterating changes the internal array pointer, resulting in elements being skipped or unexpectedly removed.

The `bug.php` file contains the problematic code. The `bugSolution.php` file provides a solution using alternative iteration methods.

This bug is subtle and can be difficult to debug, especially in larger codebases.  It's crucial to be aware of this behavior when working with associative arrays and `unset()` in PHP.