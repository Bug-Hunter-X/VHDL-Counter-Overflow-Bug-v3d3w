# VHDL Counter Overflow Bug

This repository demonstrates a common VHDL coding error: an integer counter that doesn't handle overflow correctly. The original `buggy_counter.vhdl` code increments a counter but doesn't prevent it from exceeding its defined range.  The `fixed_counter.vhdl` code shows a solution that addresses the overflow problem.

## Bug Description
The `buggy_counter` entity uses an integer signal to count. When the counter reaches 15 and increments, it wraps around to 0.  This behavior might be unexpected and could cause unforeseen issues in a larger system.

## Solution
The `fixed_counter` entity addresses the issue by adding a conditional check to stop the counter from exceeding 15.  This prevents the unexpected wrap-around behavior.
