# Uninitialized Map Access in Go

This repository demonstrates a common error in Go: accessing a key in an uninitialized map.  Go maps are not initialized by default; attempting to access a key in an uninitialized map results in a runtime panic.  The `bug.go` file shows the problematic code, while `bugSolution.go` provides a corrected version.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `go run bug.go`.
4. Observe the runtime panic.

## Solution

The solution is to explicitly initialize the map before accessing its keys.  The `bugSolution.go` file demonstrates the correct approach.

## Additional Notes

This is a common error for developers new to Go, highlighting the importance of map initialization before use.