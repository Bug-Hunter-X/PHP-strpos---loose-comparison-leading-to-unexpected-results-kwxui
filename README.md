# PHP strpos() Loose Comparison Bug

This repository demonstrates a common, yet easily missed, bug in PHP related to the use of `strpos()` with loose comparisons. The core issue stems from the fact that `strpos()` returns `false` if the substring is not found and `0` if it's found at the beginning of the string.  In loose comparisons (`==`), `false` is equivalent to `0`, leading to incorrect logic.

The `bug.php` file shows the problematic code, while `bugSolution.php` presents the corrected version.