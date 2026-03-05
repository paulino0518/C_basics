# C_basics
Some basic C notes

# Variables
int 
float
char - Single character, surrounded by single quotes

- You can declare variables first and use them later.
```
int myNum;
myNum = 15;
```
## Using variables to print an output
You can't just pass a variable like in higher level languages.  
If you do this, it will cause an error
```
int myNum = 15;
prinf(myNum);
```
To print variables in C you need to do **format specifiers**.

## Format specifiers
Used with printf, they're like a placeholder, it tells what will be printed.
Always starts with a % followed by a letter. And it is surrounded by quotes.

For integers it is d

EX:
```
int myNum = 15;
printf("%d", myNum);
```

### Common format specifiers:
- %d or %i for int
- %f or %F for float
- %lf for double
- %c for char
- %s for strings

### How to combine text and numerical format specifiers?
Put the specifier inside the text!
```
int myNum = 15;
printf("The value is: %d", myNum);
```
Example with int and char:
```
int myNum = 15;
char myLetter = 'D';
printf("My number is %d and my letter is %c", myNum, myLetter);
```

Btw you don't need to have a variable but you still need a formt specifier.

### How to declare multiple variables?
Not like i use this often but like this.  It's comma separated.
```
int x = 5, y = 3, x = 7;
//And you can assign the same value to multiple variable just like other languages
int x, y, z;
x = y = z = 50;

//This is ugly so I don't use it, i'm just writing it to internalize it's an option.
```

## Data types
**Basic data types:**
- int (2 or 4 bytes)
- float (4 bytes) - Can store 6-7 decimals
- double (8 bytes) - Can store 15 decimals
- char (1 byte)

### Characters
Stores a single character
- Surrounded by single quotes
- %c to print

Alternative:
- Use ASCII codes inside the quotes

**Reminder**: If you try to store more than one character it will only **store the last**.
For strings you need an array of characters like char myString[] = "Hello"; and use %s

### Numbers (This is where I stopped)
### Decimal Precision
### Memory size
### Extended types

## Type Conversion
