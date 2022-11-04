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
	message, err := greetings.Hello("uğur")
	if err != nil {
		fmt.Println(err)
	}
	fmt.Println(message)

	// A slice of names for Hellos func.
	names := []string{"Birdal", "Uğur", "Eren"}

	messages, err2 := greetings.Hellos(names)

	if err2 != nil {
		fmt.Println(err2)
	}

	for _, msg := range messages {
		fmt.Println(msg)
	}

}

```
add dependencies to current module and install them:

```sh
➜ go get github.com/birdalugureren/greetings
```

Let's run the code:
```sh
➜ go run hello.go
Hi, uğur. Welcome!
Hi, Birdal. Welcome!
Hi, Uğur. Welcome!
Hi, Eren. Welcome!
```
