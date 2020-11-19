# greetings
The startup application in golang that returns a greeting for the specified person.

# usage
Let's write the following code into the file named hello.go:

```go
package main

import (
	"fmt"

	"github.com/birdalugureren/greetings"
)

func main() {
	message := greetings.Hello("uğur")
	fmt.Println(message)
}

add dependencies to current module and install them:

```sh
➜ go get github.com/birdalugureren/greetings
```

Let's run the code:
```sh
➜ go run hello.go
Hi, uğur. Welcome!
```
