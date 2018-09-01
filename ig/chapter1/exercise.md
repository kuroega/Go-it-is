# Chapter 1 Exercise

2018-09-01

1. What is the whitespace?
	
	Newlines, spaces, and tabs are known as whitespaces.
	
2. What is a comment? What are the two ways of writing a comment?

	The line that starts with // is konwn as a *comment*. 
	 
	- **First** way is // comments in which all the text between the // and the end of the line is part of the comment. 
	
	- **Second** way is /* */ comments where everything between the asterisks is part of the comment (and may include multiple lines)

	
3. Our program began with `package main`. What would the files in the `fmt` package begin with?

	Files in the `fmt` package start with `package fmt`.
	
4. We used the `Println` function defined in the `fmt` package. If you wanted to use the `Exit` function from the `os` package, what would you need to do?

	Go to terminal and type `godoc os Exit`

	```go
	package main
	
	import "os"
	
	func main() {
		os.Exit(0)
	}
	```
	
5. Modify the program we wrote so that instead of printing `Hello, World` it prints `Hello, my name is ` followed by your name.

	```go
	package main
	
	import "fmt"
	
	func main() {
		name := "Rainer"
		s := fmt.Sprintf("Hello, my name is %s!", name)
		fmt.Println(s)
	}
	```