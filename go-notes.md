### programming  notes
	no parenthese around for loops or if statements
	no while loops, use fors

	for {
		// infinite for (while (true))
	}

	return multiple values from a single function (typeA, typeB)

	example fn
		func fn (x, y float64) (float64, int) {

		}
		x, y both float64
		returns two values float64, int

	defer statements defers the execution of a function until the surrounding function returns. it acts as a stack so its lifo

	there are fucking pointers...


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

