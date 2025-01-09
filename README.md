# Unreachable Code in Julia
This repository demonstrates an example of unreachable code in a Julia function. The issue arises because the function always returns a value within the if-else block, making the final return statement redundant and never executed.  This can sometimes lead to unexpected behavior or confusion when reviewing the code.

**The Bug:**
The `myfunction` in `bug.jl` contains a final `return 0` statement that will never be reached. This is a common issue when using if/else statements.  While this specific example is simple, in more complex functions this type of error can be difficult to identify.

**The Solution:**
The solution is to remove the unreachable code. The corrected code is shown in `bugSolution.jl`.