# 🤯 Brainfuck Interpreter Tutorial!

## 🔨 Setup

First, you need to install GCC (GNU Compiler Collection) to compile and run your C program!

You can download GCC from [here](https://osdn.net/projects/mingw/releases/) and watch the tutorial [here](https://youtu.be/8CNRX1Bk5sY)!

I recommend you using a code editor or an IDE such as [Visual Studio Code](https://code.visualstudio.com/) or [Visual Studio](https://visualstudio.microsoft.com/)

## 🧠 Understanding

You need to know what is Brainfuck and how it works to create an interpreter!

Brainfuck has only 8 commands: `+`, `-`, `>`, `<`, `.`, `,`, `[`, and `]`

```
>	Increment the data pointer by one (to point to the next cell to the right).

<	Decrement the data pointer by one (to point to the next cell to the left).

+	Increment the byte at the data pointer by one.

-	Decrement the byte at the data pointer by one.

.	Output the byte at the data pointer.

,	Accept one byte of input, storing its value in the byte at the data pointer.

[	If the byte at the data pointer is zero, then instead of moving the instruction pointer forward to the next command, jump it forward to the command after the matching ] command.

] If the byte at the data pointer is nonzero, then instead of moving the instruction pointer forward to the next command, jump it back to the command after the matching [ command.
```

And you can read, learn more about Brainfuck [here](https://en.wikipedia.org/wiki/Brainfuck)

## ✏️ Coding

We start by create a C file name `main.c` or any name you like

First, we include some libraries and define `MEMORY_SIZE` as 30'000

Why 30'000? Because Brainfuck has at least 30'000 or more

```
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

#define MEMORY_SIZE 30000
```
