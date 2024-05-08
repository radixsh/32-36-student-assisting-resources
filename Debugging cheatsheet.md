
# Super simple debugging cheatsheet for ECS 36a

# Compile 
Make use `-g` is included in your compilation command!!! 
## Start:  
**gdb**: `gdb program.out`
**lldb**: `lldb program.out`

## Set input file
make an input file: `example1.txt` and fill with 
```
10000
0.07
...
```
(input from the example)
This way you wont have to re-input every time you debug. 


on lldb you have to set it before you run.
**lldb**: `settings set target.input-path <input_file>`

on gdb you have to pipe input when you run
**gdb**: `run < input.txt`

## Set breaking point


**gdb**
`break linenumber`
`break filename:linenumer`

**lldb**
## Show variables 

## Show arrays/structs