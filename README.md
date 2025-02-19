# Go Race Condition in Concurrent Channel Handling

This repository demonstrates a common race condition in Go programs involving channels and wait groups.  The `bug.go` file contains the erroneous code, exhibiting a potential data race.  The `bugSolution.go` file presents a corrected version with proper synchronization mechanisms to avoid the race condition.

The issue lies in the handling of the channel and the wait group.  Understanding this problem is crucial for writing robust and reliable concurrent Go applications.

## How to reproduce

1. Clone the repository
2. Run `go run bug.go`  You might not see the error every time, because the race condition is non-deterministic.
3. Examine `bugSolution.go` to understand the correct approach.
