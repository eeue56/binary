# binary
Language inspired by whitespace and TV hackers

What if the binary dumps you see on TV were actually a programming language?


Every command begins with 16 bits and ends with 16 bits. Numbers are taken from the binary between the start and end.

The end bit pattern is a palindrome of the start bit pattern. 

## Stack

| Binary              | operation | arguments | 
|---------------------|-----------|-----------|
| 0000 0000 0000 1000 | push to top of stack      | number    |
| 0000 0000 0000 1001 | duplicate item on top of stack | n / a     |
| 0000 0000 0000 1010 | copy at a given index and put it on top of the stack      | index     |
| 0000 0000 0000 1011 | swap the two top items on the stack      | n / a     |
