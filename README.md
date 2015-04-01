# binary
Language inspired by whitespace and TV hackers

What if the binary dumps you see on TV were actually a programming language?


Every command begins with 16 bits and ends with 16 bits. Numbers are taken from the binary between the start and end.

The end bit pattern is a palindrome of the start bit pattern.

## Stack

| bit pattern         | operation                                     | arguments | 
|---------------------|-----------------------------------------------|-----------|
| 0000 0000 0000 1000 | push to top of stack                          | number    |
| 0000 0000 0000 1001 | duplicate item on top of stack | n / a        |           |
| 0000 0000 0000 1010 | copy at a given index to the top of the stack | index     |
| 0000 0000 0000 1011 | swap the two top items on the stack           |           |

## Operations


| bit pattern         | operation                                     | arguments | 
|---------------------|-----------------------------------------------|-----------|
| 0000 0000 1000 0000 | add the two top items                         |           |
| 0000 0000 1001 0000 | subtract                                      |           |
| 0000 0000 1010 0000 | multiply                                      |           |
| 0000 0000 1011 0000 | integer divide                                |           |
| 0000 0000 1000 1111 | add - take the item at index as the right hand operand | Index     |
| 0000 0000 1001 1111 | subtract - take the item at index as the right hand operand | Index     |
| 0000 0000 1010 1111 | multiply       - take the item at index as the right hand operand | Index |
| 0000 0000 1011 1111 | integer divide - take the item at index as the right hand operand | Index |
| 0000 0000 1000 1001 | add - take the item at index as the left hand operand | Index     |
| 0000 0000 1001 1001 | subtract - take the item at index as the left hand operand | Index     |
| 0000 0000 1010 1001 | multiply       - take the item at index as the left hand operand | Index |
| 0000 0000 1011 1001 | integer divide - take the item at index as the left hand operand | Index |


## I/O

| bit pattern         | operation                                     | arguments | 
|---------------------|-----------------------------------------------|-----------|
| 0000 1000 0000 0000 | print number at top of stack                  |           |
| 0000 1001 0000 0000 | print char at top of stack                    |           |
| 0000 1010 0000 0000 | read number to top of stack                   |           |
| 0000 1011 0000 0000 | read char to top of stack                     |           |
