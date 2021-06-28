# Brainfuck Demo

## Intro

Brainfuck is an esoteric programming language with 8 very simple instructions created by Urban Müller. His aim was to create a Turing-complete language for which he can write the smallest compiler ever. His compiler was 240 bytes in size and later he had managed to bring it under 200 bytes.

The 8 operators that are used in the language are `<>+-[],.`. Even with these 8 operators a person is capable of writing almost any program that he can think of.

Below are the working of the above operators.

```brainfuck
> = Increment the pointer.
< = Decrement the pointer.
+ = Increment the byte at the pointer.
- = Decrement the byte at the pointer.
[ = Jump forward past the matching ] if the byte at the pointer is zero.
] = Jump backward to the matching [ unless the byte at the pointer is zero.
, = Input a byte and store it in the byte at the pointer.
. = Output the byte at the pointer.
```

## Modules Used

- node-brainfuck


## Installation / Setup


```bash
npm install
```

## Usage

Run the application by using node.

```bash
node app.js
```

Output
```bash
MY NAME IS FAISAL
```
Simple format
```
//This is the representation of brainfuck code with individual character in each line.
//Every line over here generates an ASCII value and ASCII value represents a character.

>+++++++[>+++++++++++<-]>.          <!-- ASCII - 77, Char - 'M' --->
<<>+++++[>++<-]>++.                 <!-- ASCII - 89, Char - 'Y' --->

>.                                  <!-- ASCII - 0, Char - ' ' --->

<<<>+++++[>--<-]>-.                 <!-- ASCII - 78, Char - 'N' --->
<<>+++++[>--<-]>---.                <!-- ASCII - 65, Char - 'A' --->
<<>+++++[>++<-]>++.                 <!-- ASCII - 77, Char - 'M' --->
<<>+++++[>--<-]>++.                 <!-- ASCII - 69, Char - 'E' --->

>.                                  <!-- ASCII - 0, Char - ' ' --->

<<<>++[>++<-]>.                     <!-- ASCII - 73, Char - 'I' --->
<<>++[>+++++<-]>.                   <!-- ASCII - 83, Char - 'S' --->

[-].                                <!-- ASCII - 0, Char - ' ' --->

>+++++++[>++++++++++<-]>.           <!-- ASCII - 70, Char - 'F' --->
-----.                              <!-- ASCII - 65, Char - 'A' --->
++++++++.                           <!-- ASCII - 73, Char - 'I' --->
<<>+++++[>++<-]>.                   <!-- ASCII - 83, Char - 'S' --->
<<>+++[>------<-]>.                 <!-- ASCII - 65, Char - 'A' --->
<<>++[>+++++<-]>+.[-].              <!-- ASCII - 76, Char - 'L' --->
```

## Resource
[Basic guide](http://www.muppetlabs.com/~breadbox/bf/)\
[Detailed guide](https://gist.github.com/roachhd/dce54bec8ba55fb17d3a)