# Byte Print

convert byte size into human readable format in Go.

## Download
`go get github.com/twiny/bprint`

## Example

```go
package main

import (
	"fmt"
	"runtime"

	"github.com/twiny/bprint"
)

func main() {
	stats := new(runtime.MemStats)
	runtime.ReadMemStats(stats)
	//
	fmt.Println(bprint.String(stats.Sys))
}

// output
// 68.08M
```