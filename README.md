# Nil Map Panic in Go

This repository demonstrates a common error in Go: panicking due to accessing a nil map.  Go maps are not automatically initialized; attempting to access a key in a nil map will result in a runtime panic.

The `bug.go` file contains code that reproduces this issue.  The `bugSolution.go` file shows the correct way to handle this by checking for nil before accessing the map.

This is a crucial concept for robust Go programming. Always check for `nil` before using maps (and other references) to avoid unexpected crashes.