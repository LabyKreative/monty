# The Monty Language

![alt text](https://live.staticflickr.com/3173/2962153608_8d57aaf8aa_b.jpg)

## Description

Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

***

## Installation

Make this repo yours by cloning it:
```console
https://github.com/LabyKreative/monty.git
```

1. Compile:
```console
gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty
```

2. Execute:
```console
./monty file.m
//The file contains the bytcode instructions e.g.
cat -e 000.m
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

## Functions

The functions used are:

|Name | Description | Return| File
|:--: | :-- | :--| :--|
|_f_add | adds the top two elements of the stack | No Return | add.c|
| addnode | add node to the head stack | No Return | addnode.c|
| f_div | divides the top two elements of the stack. | No Return | div.c|
| execute | executes the opcode | No Return | execute.c|
| free_stack | frees a doubly linked list | No Return | free_stack.c|
| main | monty code interpreter | 0 on success | main.c| 

### Examples

```console
$labykreative> ls
basics.c    general.c  main.h  memory.c   shell.c
builders.c  helper.c   hsh          README.md  test
```

### Authors
[Adeyemi Owolabi](https://github.com/LabyKreative) and [Engr. Princess Khumbize Chimsale](https://github.com/Khumbize)
