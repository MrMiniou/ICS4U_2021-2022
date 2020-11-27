## Note – Stacks

The **stack** is an abstract data type that is a collection of elements that are "stacked" on top of each other. Elements get added and removed from the top of the stack. The stack ADT is also known as LIFO (last in, first out) system. 

These are some the typical operations of a stack ADT.

* retrieve the item at the top of the stack
* remove the item at the top of the stack
* add an item to the top of the stack
* check whether the stack is empty

An example of a usage of the stack ADT is your browser history. Every time you visit a new webpage, it gets added to the top of your browser history. Every time you hit "back", it removes the webpage you were just at from the stack, and brings you back to the most previously visited webpage. Of course, you can jump back more than one page at once, which a stack doesn't have to do, but the basic operations of web browsing follow a stack ADT.

Java has a class called `Stack`. You need to import `java.util.Stack` in order to use it. Here are some of its methods. 

| Method    | Explanation                                                  | Example                                      | Explanation                                                  |
| --------- | ------------------------------------------------------------ | -------------------------------------------- | ------------------------------------------------------------ |
| `Stack()` | Creates a new (empty) stack.                                 | `Stack<Integer> stackExample = new Stack();` | Creates a new stack of integers called `stackExample`. It is initialized to the empty stack. |
| `empty()` | Returns `true` if the stack is empty, and `false` otherwise. | `stackExample.empty()`                       | Returns `true`, since `stackExample` is currently empty.     |
| `push()`  | Adds an elements to the top of the stack. Throws `EmptyStackException` if the stack is empty. | `stackExample.push(1234)`                    | Adds `1234` to the top of `stackExample`.                    |
| `peek()`  | Returns the top element. Throws `EmptyStackException` if the stack is empty. | `stackExample.peek()`                        | Returns  `1234`.                                             |
| `pop()`   | Removes the top element. Throws `EmptyStackException` if the stack is empty. | `stackExample.pop()`                         | Removes the top element. Now, `stackExample` is empty again. |

The `Stack` class is integrated using the `Vector` class, so you can also use any methods from `Vector` on a `Stack` object. 
