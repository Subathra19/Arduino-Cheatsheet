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
```c
sizeof() //unary operator used to compute the size of its operand (i.e) returns the amount of memory allocated
```
### Numeric Constants
```c
HIGH | LOW
INPUT | OUTPUT
156        // decimal
0b00110011 // binary
0267       // octal
0xC8       // hexadecimal
10U        // force unsigned
10L        // force long
10UL       // force unsigned long
10.0       // force floating point
10.2e6     // 10.2*10^6 = 1230000
```

### Data types
```c
bool          // true or false
char          // -128 to 127, 's','@'
unsigned char // 0 to 255
byte          // 0 to 255
int           // -32768 to 32767
unsigned int  // 0 to 65535
word          // 0 to 65535
long          // -2147483648 to 2147483647
unsigned long // 0 to 4294967295
float         // -3.4028e+38 to 3.4028e+38
double        // -3.4028e+38 to 3.4028e+38
void          // no return value
```
### Array
```c
int a[]={10,20,30};
int a[5]={1,2,3,4,5};
int a[5];
```

### Strings
```c
char a[6] = {'H','e','l','l','o','\0'};
char a[6] = {'H','e','l','l','o'};
char a[6] = {"Hello"};
char a[] = {"Hello"};
```
### Qualifiers
```c
static   // preserves the value even when they are out of their scope
volatile // in RAM (nice for ISR)--> to tell the compiler, that the value may change at any time.
const    //read-only
PROGMEM  //in flash memory
```
### Built-in Functins
* Digital I/O
```c
//Digital I/O pins: 0-13 
 pinMode(pin,[INPUT, OUTPUT, INPUT_PULLUP])
 int digitalRead(pin)
 digitalWrite(pin, [HIGH, LOW])
```
* Analog I/O
```c
//Analog I/O pins: A0-A5
pinMode(pin,[INPUT, OUTPUT, INPUT_PULLUP])
int analogRead(pin)
analogWrite(pin, value) // PWM Out pins: 3 5 6 9 10 11
analogReference([DEFAULT, INTERNAL, EXTERNAL])
```
