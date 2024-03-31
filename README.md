# 0x19. C - Stacks, Queues - LIFO, FIFO
# Monty
## Compilation & Output
* Your code will be compiled this way:
```
$ gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty

```
## Monty byte code files

Files containing Monty byte codes usually have the .m extension. Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument:

```
 push 0$
push 1$
push 2$
  push 3$
                   pall    $
push 4$
    push 5    $
      push    6        $
pall$

```

# Usage

All the files are compiled in the following form:

```
 gcc -Wall -Werror -Wextra -pedantic *.c -o monty.

```

To run the program:

```
 ./monty bytecode_file
```
Available operation codes:
```
# push  |Pushes an element to the stack. e.g (push 1 # pushes 1 into the stack)|
# pall  |Prints all the values on the stack, starting from the to of the stack.|
#pint   | Prints the value at the top of the stack.|
#pop    | Removes the to element of the stack. |
#swap   | Swaps the top to elements of the stack.|
#add    | Adds the top two elements of the stack. The result is then stored in the second node, and the first node is removed.|
#nop    | This opcode does not do anything.|
#sub    | Subtracts the top two elements of the stack from the second top element. The result is then stored in the second node, and the first node is removed.|
#div    | Divides the top two elements of the stack from the second top element. The result is then stored in the second node, and the first node is removed.|
#mul    | Multiplies the top two elements of the stack from the second top element. The result is then stored in the second node, and the first node is removed.|
#mod    | Computes the remainder of the top two elements of the stack from the second top element. The result is then stored in the second node, and the first node is removed.|
#       | When the first non-space of a line is a # the line will be trated as a comment.|
#pchar  | Prints the integer stored in the top of the stack as its ascii value representation.|
#pstr   | Prints the integers stored in the stack as their ascii value representation. It stops printing when the value is 0, when the stack is over and when the value of the element is a non-ascii value.|
#rotl   | Rotates the top of the stack to the bottom of the stack.|
#rotr   | Rotates the bottom of the stack to the top of the stack.|
#stack  | This is the default behavior. Sets the format of the data into a stack (LIFO).|
#queue  | Sets the format of the data into a queue (FIFO).|
```
# AUTORS
```
 Yonas G/hiwot   : yonihabeshaw@gmail.com 
 Dagmawit Terefe : dagm24b@gmail.com
```
