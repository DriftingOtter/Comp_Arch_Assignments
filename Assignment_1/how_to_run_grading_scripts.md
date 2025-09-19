# How To Run Grading Script

Unzip tar file
```Bash
$ tar -xf pa1-grader.tar
```

Contains python script(s)
```Bash
$ ls
autograde.py   /data    grader.py
```

```
$ mkdir src/rot13

    !--- make code, DONT COMPILE --!

$ chmod +x rot13.c
```

make the code. 

```
$ ./grader.py rot13
```

It will create a build directory and compile the code and run it on the 50/100 
test cases provided.

## Addional Things

This will compile the updated version of the code from the makefile.
```
$ cd /build
$ make
```

# Tips

- Make sure the input for each program from the correct stream (argv, stdin, file, etc.)

## Reading from file {fscanf()}

- Make sure you provide the correct format specifier to what value you are 
  expecting, and a valid twin pointer variable to store to

- When `fscanf()` returns **-1** if it finds a byte that is not the specified one.

### Format Specifiers

i or d : integer
u : unsigned integer
x : hex integer
o : octal integer
f : floating point number
lf: double point number
c : character

s[width][length] : string *(ALWAYS MAKE SURE YOU PROVIDE THE LENGTH)*


