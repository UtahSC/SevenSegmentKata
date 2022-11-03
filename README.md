# Seven Segment Display Kata

A seven segment display is one of the earliest digital displays. 
It consists of a set of two vertical segments, three horizontal segments, and two more vertical segments, arranged to make two stacked boxes like so:

```
 _ 
|_|
|_|
```

By turning the correct segments off and on, it is possible to display a representation of the digits 0-9 using only these seven elements.

In this kata, we'll practice transforming a number into it's seven-segment display representation.

## Step 1: Single digit numbers

Write a function that takes a single digit number and returns a string that can be written to the console.
To represent a seven-segment display in text we need three lines, but your function should only return one string, so make sure that you include line breaks.
Here are the numbers 0-9 (to keep the display manageable, I've concatenated them in this example, but in this step you only need to return a single digit.

```
 _     _  _     _  _  _  _  _ 
| |  | _| _||_||_ |_   ||_||_|
|_|  ||_  _|  | _||_|  ||_| _|
```

## Step 2: Multi-digit numbers

Improve your function so that it can handle arbitrary length integers.
For now, assume that your console has infinite width.

## Step 3: Wrapping

Unfortunately, infinite width display technology is not yet particularly affordable, so we need to wrap at some point.
Limit the width of your output to 10 digits, so 12345678901 will be rendered as:

```
    _  _     _  _  _  _  _  _ 
  | _| _||_||_ |_   ||_||_|| |
  ||_  _|  | _||_|  ||_| _||_|
  
  |
  |
```
