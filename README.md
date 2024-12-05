# Subtle Memory Management Bug in Objective-C

This repository demonstrates a common, yet easily overlooked, memory management error in Objective-C related to the improper use of `retain`, `release`, and `autorelease`.  The bug is subtle and can lead to crashes or memory leaks that are difficult to track down.

## Bug Description
The `bug.m` file contains code that incorrectly handles memory management for an NSString property.  The solution is presented in `bugSolution.m`.

## How to Reproduce
1. Clone this repository.
2. Open the project in Xcode.
3. Run the application.  Observe the potential crash or memory leak.
4. Compare the buggy code (`bug.m`) to the corrected code (`bugSolution.m`).

## Solution
The solution involves correctly managing the memory lifecycle of the NSString property.  Modern Objective-C (using ARC) largely avoids this issue, however the understanding of the concepts remains important. 