### online playground
	http://play.golang.org/
	
### file layout
	package <i>name</i>

	import (
		"<i>package1</i>"
		"<i>package2/sub</i>"
	)

### function definitions
	return multiple values from a single function (typeA, typeB)

		func fn (x, y float64) (float64, int) {

		}

		x, y both float64
		returns two values float64, int

	named return values (only use in obvious situations)
		func fn2 (x float64, y int) (a, b int) {
			a = 1
			b = 2
			return
		}

### variables
	variables can be declared at the function level or the package level.
	variables can be initialized upon declaration
	multiple variables can be declared at once if they are of the same type
	initializers are applied based upon position
	if a variable is not initialized, it is the default value "zero" value for that type.
	a variable's var and type can be omitted if the type is obvious based upon the declaration (k below will be an int)
	one variable can be cast to another type, but only explicitly (u and f below)


	package me

	var x, y, z int = 1, 2, 3

	func fn (a int) (int) {
		k := 3
		u := uint(k)
		f := float64(u)

		return x + y + z + a
	}

### concurrency
	defer statements defers the execution of a function until the surrounding function returns. it acts as a stack so its lifo


### looping
	no parenthese around for loops or if statements
	manadatory brackets {}
	no while loops, use fors

	for {
		// infinite for (while (true))
	}

### if / thens
	no parenthese around if statements
	manadatory brackets {}
	like we're used to in for loops, there can be a little short statement at the beginning of an if statement or a switch statement. 
	the values of those little short statements are available throughout the if ladder

	func fn (x int) {}
		if k:=3+x; k<10 {
			return k
		} else {
			return k - 10
		}
	}

	there are fucking pointers...

### fmt library
* used to print stuff out
* import "fmt"


### Compilation
* go build x.go
	- builds x.go to x
	- run ./x

* go build x.go packages.go

### go get
* go get github.com/mailgun/godebug
	- installs the godebug library
	- will install godebug's src and its bin

### Debugging
* use mailgun's godebug. introduced in 1/2015 so pretty new. before that it was gdb.
	- https://github.com/mailgun/godebug
* go get github.com/mailgun/godebug
	- installs the godebug library
* insert a '_ = "breakpoint"' to get a breakpoint going
* godebug run x.go
	- starts the debugger for x; stopping at the first breakpoint

