# Arduino-Cheatsheet
* It includes the basic syntax and built in functions for Arduino programmers
### 1. Sketch
* Structure of the program
```c
void setup(){
	//Runs only once and initiates the variables
}
Void loop{
	// Runs repeatedly and controls the board
}
```
* Functions
```c
<return type> <name>(<params>) { ... } //syntax
int sum(int x,int y) {return x+y;} //example
//Return types
return x; // x must match return type
return; // For void return type
```
### 2. Control Structures
```c
//Conditional statement
if<condition>{ <statement> }else{ <statement> }

//Loops
while (<condiiton) { <statement> }

do{ <statement> }(<condiiton)// condition is tested at the end of loop 
for (initialization expression; condition for expression; update expression){    
	// body of the loop
}

//Loop control statement
break; // Exit a loop immediately
continue; // Go to next iteration

switch(var){
 case 1:
 <statement>
 break;
 case 2:
 <statement>
 break;
 default:
 <statement>
}
```
### 3. operators
* Arithmetic
```c
= //assignment
+ //add
- //subtract
* //multiply 
/ //divide
% //modulo
```
* Comparison
```c
== //equal to
!= //not equal to
<  //less than 
>  //greater than
<= //less than or equal to
>= //greater than or equal to
```
* Boolean
```c
&& // and
|| // or
!  // not
```
* Bitwise
```c
&   //bitwise and 
|   //bitwise or
^   //bitwise xor 
~   //bitwise not
<<  //shift left 
>>  //shift right
```
* Compound 
```c
++ //increment
-- //decrement
+= //compound addition
-= //compound subtraction
*= //compound multiplication
/= //compound division
&= //compound bitwise and
|= //compound bitwise or
```
* Pointer access
```c
& //reference: get a pointer
* //dereference: follow a pointer
```


