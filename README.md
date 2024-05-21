# Go Language Basics (Part 1)

Let's now familiarize ourselves with the basic types and constructs that Go offers by diving into an exercise.

## Go Proverbs

The next exercise will make use of a set of sayings (proverbs) that the Go community take to heart when working with the language. These proverbs originate from a [conference talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) given by one of the creators of the language, Rob Pike.

```
Don't communicate by sharing memory, share memory by communicating.
Concurrency is not parallelism.
Channels orchestrate; mutexes serialize.
The bigger the interface, the weaker the abstraction.
Make the zero value useful.
interface{} says nothing.
Gofmt's style is no one's favorite, yet gofmt is everyone's favorite.
A little copying is better than a little dependency.
Syscall must always be guarded with build tags.
Cgo must always be guarded with build tags.
Cgo is not Go.
With the unsafe package there are no guarantees.
Clear is better than clever.
Reflection is never clear.
Errors are values.
Don't just check errors, handle them gracefully.
Design the architecture, name the components, document the details.
Documentation is for users.
Don't panic.
```

> :bulb: Treat the whole set of proverbs as a single newline-delimited raw string literal and store it in a constant before you start working with it. See [spec](https://golang.org/ref/spec#String_literals) for more on string literals in Go.

## Exercise

Given the newline-delimited proverbs string, count the number of words that appear on each line.

### What you need to know

- [Values](https://gobyexample.com/values)
- [Variables](https://gobyexample.com/variables)
- [Constants](https://gobyexample.com/constants)
- [For](https://gobyexample.com/for)
- [If/Else](https://gobyexample.com/if-else)
- [Switch](https://gobyexample.com/switch)
- [Arrays](https://gobyexample.com/arrays)
- [Slices](https://gobyexample.com/slices)
- [Range](https://gobyexample.com/range)

> :bookmark: You will also find the [Strings, bytes, and runes](https://blog.golang.org/strings) blog post useful for understanding how Go treats strings.

### Success Criteria

Your program output should look like the following:

```
1. Don't communicate by sharing memory, share memory by communicating. (WC: 9)
2. Concurrency is not parallelism. (WC: 4)
3. Channels orchestrate; mutexes serialize. (WC: 4)
4. The bigger the interface, the weaker the abstraction. (WC: 8)
5. Make the zero value useful. (WC: 5)
6. interface{} says nothing. (WC: 3)
7. Gofmt's style is no one's favorite, yet gofmt is everyone's favorite. (WC: 11)
8. A little copying is better than a little dependency. (WC: 9)
9. Syscall must always be guarded with build tags. (WC: 8)
10. Cgo must always be guarded with build tags. (WC: 8)
11. Cgo is not Go. (WC: 4)
12. With the unsafe package there are no guarantees. (WC: 8)
13. Clear is better than clever. (WC: 5)
14. Reflection is never clear. (WC: 4)
15. Errors are values. (WC: 3)
16. Don't just check errors, handle them gracefully. (WC: 7)
17. Design the architecture, name the components, document the details. (WC: 9)
18. Documentation is for users. (WC: 4)
19. Don't panic. (WC: 2)
```

> :bulb: Use the `strings` package and find the appropriate function that helps you split your lines into words.

## Assignment Submission
* [ ] Create a separate branch named `solution` in which to do your work.
* [ ] Create a `cmd/proverbcounter` folder with a `main.go` file containing your solution.
* [ ] A PR will automatically be opened when you push your `solution` branch to GitHub. Instructor will provide feedback in that PR.
