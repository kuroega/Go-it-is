# Chapter 2 Types

1. How are integers stored on a computer?
	
	They are stored as base 2 numbers.
	
2. We know that (in base 10) the largest one-digit number is 9 and the largest two-digit number is 99. Given that in binary three-digit number is 111(7) and the largest four-digit number is 1111(15), what's the largest eight-digit number? 
	
	11111111(255)
	
3. Although overpowered for the task, you can use Go as a calculator. Write a program that computes 32,132 x 42,452 and prints it to the terminal (use the * operator for multiplication)

	```go
	package main
	
	import "fmt"
	
	func main() {
		fmt.Println("32,132 x 42,452 = ", 32132 * 42452)
	}
	```
	
4. What is a string? How do you find its length?
	
	string a sequence of characters with definite length. The length is found by calculating each of its characters (i.e., one character represents one unit of length)

5. What's the value of the expression `(true && false) || (false && true) || !(false && false) ?`
	true