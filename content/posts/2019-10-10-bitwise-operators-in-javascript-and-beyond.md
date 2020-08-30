---
title: "Bitwise operators in JavaScript and beyond"
summary: ""
photo: 2019-10-10.jpg
draft: true
---

We (humankind) tend to use the decimal numeral system (base-10). Computers deeply are significantly less complex than people because they operate using binary numeral system (base-2). Central processing unit (CPU) of every single computer is made of gazillion transistors and they can store only `0` or `1`. The smallest computing unit that describes if the transistor is on or off is a [Bit](https://en.wikipedia.org/wiki/Bit). By itself a bit isn't too comprehensive, but more complex information units like [Byte](https://en.wikipedia.org/wiki/Byte) allow us to store a lot more data variations (256 to be precise).

<!-- What are bitwise operators and why people should carry on reading -->

Although JavaScript being high-level programming language doesn't often require developers to care about such a low-level details, having a basic grasp of it may put your software development skills to the next level. Let's explore the power of bitwise operators and present few practical use cases using JavaScript language. Before that let's cover a necessary prerequisite.

## Numeral Systems

What if I told you that `10010011`, `147` and `93` represent exactly the same value? Thats right, the only difference is the numeral system. [Radix](https://en.wikipedia.org/wiki/Radix), commonly referred as a "base", is the number of unique symbols used to represent a numeral value in [positional  numeral systems](https://en.wikipedia.org/wiki/Numeral_system#Positional_systems_in_detail). Let me go through few commonly used in software development and real life. 

### Decimal Numeral System (Base-10)

What is the easiest way of representing a numeral value? Of course — using your fingers! That is most likely the reason why [decimal numeral system ](https://en.wikipedia.org/wiki/Decimal) became the most popular one since the age of ancient civilizations. Although I mentioned that computers deeply operate using binary values only, numeric values are usually converted to decimal representation for the end user convenience.

<iframe src="https://codesandbox.io/embed/mystifying-antonelli-vsvn2?fontsize=14&hidenavigation=1&view=preview&runonclick=0" title="2019-09-26-base-10" allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb" style="width:100%; height:468px; border:0; border-radius: 4px; overflow:hidden;" sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"></iframe>

### Hexadecimal Numeral System (Base-16)

Hexadecimal (derived from the hex for "six" and decimal for "tenth") is composed of sixteen unique symbols, `0-9` to represent a value between zero and nine and `a-f` to represent values between ten and fifteen. This notation has broad application in computer science because single symbol represent a human readable format of [binary nibble](https://en.wikipedia.org/wiki/Nibble). In C-like programming languages (C, C++, C#, Java, JavaScript, Python etc.) `0x` prefix is used to represent hexadecimal notation. [Hex triplets](https://en.wikipedia.org/wiki/Web_colors#Hex_triplet) are commonly used to define color values.

<iframe src="https://codesandbox.io/embed/2019-09-26-base-16-wsxvt?fontsize=14&hidenavigation=1&view=preview&runonclick=0" title="2019-09-26-base-10" allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb" style="width:100%; height:468px; border:0; border-radius: 4px; overflow:hidden;" sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"></iframe>

### Binary Numeral System (Base-2)

Represented using sequences of bits binary system is used under the hood almost by ever computer-based device. Back in the days simple switches or punched holes, nowadays two different voltages on microscopic transistors store binary values. Written using `0` and `1` symbol seems to be the most popular convention within mathematicians and computer scientists crowd.

<iframe src="https://codesandbox.io/embed/2019-09-26-base-16-byyer?fontsize=14&hidenavigation=1&view=preview&runonclick=0" title="2019-09-26-base-10" allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb" style="width:100%; height:468px; border:0; border-radius: 4px; overflow:hidden;" sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"></iframe>
