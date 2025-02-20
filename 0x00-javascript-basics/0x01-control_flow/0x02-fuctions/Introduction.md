# Introduction
Control Flow refers to the order in which statements and instructions are executed in a program
By default, JavaScript code runs line by line from top to bottom, but control flow structures allow us to alter this execution.
## Classification of control flows
### Conditionals
Conditionals allow you to execute different blocks of code based on specific conditions.
#### if statement﻿
The if statement is used to execute a block of code if a specified condition is true.

The syntax is as follows:

if (condition) {
  // block of code to be executed if the condition is true
}
#### if else statement﻿
Executes the code in the if block when the condition is true, if the condition is false, the code inside the else block gets executed.

if (condition) {
  // block of code to be executed if the condition is true
} else {
  // block of code to be executed if the condition is false
}
#### if else ladder
Used when multiple conditions need to be checked sequentially.

The syntax is as follows:

if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if condition1 is false and condition2 is true
} else {
  // block of code to be executed if both condition1 and condition2 are false
}
#### Switch Statement﻿
Used when a variable has multiple possible values. It’s cleaner than multiple if..else if conditions.

The syntax is as follows:

switch (expression) {
  case value1:
    // block of code to be executed if expression === value1
    break;
  case value2:
    // block of code to be executed if expression === value2
    break;
  default:
  // block of code to be executed if expression doesn't match any case
}
#### Ternary Operator﻿
The ternary operator provides a concise way to write if-else statements in a single line.

The syntax is:

condition ? expression if condition is true : expression if condition is fal
### Loops
#### for loop﻿
Used when the number of times the block of code should be executed is known.

The syntax is as follows:

for (initialization; condition; update) {
    // code
}
Initialization is used to initialize the variable used in the loop.

Condition is used to evaluate the condition of the initial variable, if the condition returns true, the loop starts over again, if the condition returns false, the loop ends.

Update is used to update the initialization variable.
#### while loop﻿
Runs as long as a specified condition remains true.

while (condition) {
  // code block to be executed if condition is true
}
#### do while loop﻿
Executes the loop at least once, even if the condition is false from the start.

do {
  /* code of block that will be
     executed at least once even if
     condition is false */
} while (condition);
#### break and continue statements﻿
break and continue statements are keywords that are always used within a loop
##### break statement﻿
The purpose of a break statement is used when we want to terminate the running loop whenever any particular condition occurs.

Whenever a break statement occurs, the loop breaks and stops executing.

The break statement exits the loop completely.

for (let i = 0; i < 10; i++) {
  if (i == 5) {
    break;
  }
  console.log(i);
}
#### continue statement﻿
++++++=+=The continue statement is used when we want to skip a particular iteration.

Whenever we write continue statement, the whole code after that statement is skipped and the loop will go for the next iteration.

The continue statement skips the current iteration and moves on to the next iteration.

for (let i = 0; i < 10; i++) {
  if (i == 5) {
    continue;
  }
  console.log(i);
}
