# Rust Undefined Behavior Example
This repository demonstrates a common source of undefined behavior in Rust: modifying a vector through a raw pointer after the vector's allocation may have changed.  The code in `bug.rs` exhibits this behavior, leading to unpredictable results. The solution in `bugSolution.rs` provides a safer alternative.

## How to reproduce
1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `rustc bug.rs` and `./bug`.
4. Observe the unpredictable output.
5. Compare the output with the corrected version in `bugSolution.rs`.