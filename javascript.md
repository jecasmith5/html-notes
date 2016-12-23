#chapter 1

Values,types and operators

Data-read,modify,create

bits-zeros and ones

high-low strong-weak shiny-dull

values-chunks of bits containing info

####numbers-numeric values

13

9.81

2.998e8(2.998 x 10^8=299,800,000)

use for arithmatic:add,subtract,multiply,devide

+*-/operators*

% remainder operator modulo

remainder of x/y

infinity,-infinity

NaN-not a number

####strings

text "this is a string"

escaping a character-use \ character after has special meaning

\n-newline

strings can only use the + operator to concatenate(glue two strings together)

Unary Values-console.log-shows on screen

####booleans

yes/no on/off TRUE/FALSE

!= not equal ==equal

NaN==NaN is FALSE

&& and true only if both are TRUE

|| or true if either are true

! Not

####objects

####functions

####undefined values

null and undefined-absense of meaningful value

type coercion, if wrong type of value converts to type it wants

#chapter2

####Program structure

fragment of code that produces value-expression

always use semicolons at end of lines

####Variables

to catch and hold values

var caught = 5*5;

var name = expression

after defined you can use it as an expression

var ten=10;
console.log(ten * ten)
// 100

no spaces,cant start with a numbers,no punctuation

####keywords and reserved words

break case catch class const continue debugger

default delete do else enum export extends false

finally for function if implements import in

instanceof interface let new null package private

protected public return static super switch this

throw true try typeof var void while with yield

cannot be used as var name

####functions

alert-pop up box

alert("Goof morning!");

invoking calling or applying functions

values given-arguments

Command-Option-i pulls up console

####Return values

math.max takes any number of number values and give back the greatest

console.log(Math.max(2,4));
// 4

console.log(Math.max(2,4)+100);
//102

####Prompt and confirm

ask the user to ok/cancel

confirm("shall we,then?");

prompt asks open question:

prompt("tell me everything you know","...");

####Control Flow

top to bottom

conditional execution-if keywords

if and only if

if/else

####while and do loops

loop:way to repeat

indenting code

for loops

switch

switch (prompt("What is the weather like?")) {
  case "rainy":
    console.log("Remember to bring an umbrella.");
    break;
  case "sunny":
    console.log("Dress lightly.");
  case "cloudy":
    console.log("Go outside.");
    break;
  default:
    console.log("Unknown weather type!");
    break;
}

variable names

fuzzylittleturtle
fuzzy_little_turtle
FuzzyLittleTurtle
fuzzyLittleTurtle-most used

//comments

triangle loop

for (var triangle = "#"; triangle.length < 8; triangle += "#")
  console.log(triangle);

fizzbuzz

for(var i=1;i<=100;i++){
  var answer="";
  if(i % 3 == 0)
  answer +="Fizz"
  if(n % 5 == 0)
  answer =="Buzz"
  console.log(answer||i);
}
  )
#Chapter 3

####functions

funcions have a set of parameters and a body

can have multiple parameters or none

none:

var makeNoise = function() {
  console.log("Pling!");
};

makeNoise();
// → Pling!

multiple:

var power = function(base, exponent) {
  var result = 1;
  for (var count = 0; count < exponent; count++)
    result *= base;*
  return result;
};

console.log(power(2, 10));
// → 1024

parameters and scopes:

local to the function meaning they cant be used throughout Program

outside of function-global

####Nested scopes

if a function is outside of local scope it wont be seen by the oter functions

functions as values:

var launchMissiles = function(value) {
  missileSystem.launch("now");
};
if (safeMode)
  launchMissiles = function(value)

declaration notation

shortcut to var square=function

function square(x){
  return x * x;
}

The call stack:

top
   greet
        console.log
   greet
top
   console.log
top

out of stack space or too much recursion

Optional arguments:

If you pass too many, the extra ones are ignored.

If you pass too few, the missing parameters simply get assigned the value undefined.

wrapValue-which creates a local variable.returns a function that accesses and returns this local variable.

closure-reference specific of local variables in an enclosed function

recursion-function that calls intself

functions and side effects:

prints line, returns values

pure-no side effects

#chaper 4
