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

objects and arrays

objecs-group values including other objects

WERESQUIRREL

data structure-stores information in sets

array-list of values between [] separated by commas

var listOfNumbers = [2, 3, 5, 7, 11];

starts at 0

listOfNumbers[0]=2

properties

accesse properties .x of value[x]

toUpperCase-convert to uppercase

toLowerCase-convert to lower

properties that contain functions-methods

push-add values to end of array-list

pop-removes values

join-array of strings can be made into single string

####objects

collections of properties can add and remove these properties
{}

  var descriptions = {
  work: "Went to work",
  "touched tree": "Touched a tree"
};

deletes-cuts off from tentacle

in-returns booleen value

####mutabiity

immutable-impossible to changean existing value

string that contains "cat", it is not possible for other code to change a character in that string to make it spell "rat".

objects, content of value can be modified by changing properties

####lycannthropes log

correlation-measure of dependence between variables

-1 to 1

ϕ =
n11n00 - n10n01
√ n1•n0•n•1n•0

####Objects as maps

name and value properties

square bracket access notation to create and read the properties and can use the in operator to test whether a given property exists.

var map = {};
function storePhi(event, phi) {
  map[event] = phi;
}

map-way to change domains

####Arrayology

unshift and shift add or remove at start of Array

add task to end of list-rememberTo

ready to do something-whatIsNext

get and removes item from front of list

indexOf(front of list)

lastIndexOf-end of list

slice-only whats in between start and finish

function argumentCounter() {
  console.log("You gave me", arguments.length, "arguments.");
}
argumentCounter("Straw man", "Tautology", "Ad hominem");
// → You gave me 3 arguments.

####Math

Math.max (maximum)

 Math.min (minimum)

 Math.sqrt (square root).

cos (cosine), sin (sine), and tan (tangent)

inverse

acos, asin, and atan

Math.PI-pi

math.random--gives random number between 0 and 1

math.floor rounds number down

math.ceil rounds number up

#Chapter5

####Abstraction

hide details and give us ability to talk at higher level

insteaad of uw=sing a million

for() create a function

function logEach(array) {
  for (var i = 0; i < array.length; i++)
    console.log(array[i]);
}

.forEach

####Higher order functions

rely on other functions

functions that create new functions

functions that change other functions

apply

####json

JavaScript Object Notation. It is widely used as a data storage and communication format on the Web.

fitering an array-builds new array based on conditions

####Transforming with map

transforms an array by applying a function to all of its elements and building a new array from the returned values

composability

compose into concepts to write clear

Binding

creates new function that calls original function

#Chapter 6

complexity made easier by separating into compartments

objects are compartments

methods present interface of how object is used

encapsulation (distinguishing between internal complexity and external interface)

####methods

properties that hold function values

var rabbit = {};
rabbit.speak = function(line) {
  console.log("The rabbit says '" + line + "'");
};

rabbit.speak("I'm alive.");
// → The rabbit says 'I'm alive.'

object.method()

function speak(line) {
  console.log("The " + this.type + " rabbit says '" +
              line + "'");
}
var whiteRabbit = {type: "white", speak: speak};
var fatRabbit = {type: "fat", speak: speak};

whiteRabbit.speak("Oh my ears and whiskers, " + "how late it's getting!");
// → The white rabbit says 'Oh my ears and whiskers, how
//   late it's getting!'
fatRabbit.speak("I could sure use a carrot right now.");
// → The fat rabbit says 'I could sure use a carrot
//   right now.'

####prototypes

var empty = {};
console.log(empty.toString);
// → function toString(){…}
console.log(empty.toString());
// → [object Object]

When an object gets a request for a property that it does not have, its prototype will be searched for the property, then the prototype’s prototype, and so on.

Functions derive from Function.prototype, and arrays derive from Array.prototype

Object.getPrototypeOf function obviously returns the prototype of an object

#constructors

create objects that derive from shared prototypes

Constructors (in fact, all functions) automatically get a property named prototype

Rabbit.prototype.speak = function(line) {
  console.log("The " + this.type + " rabbit says '" +
              line + "'");
};
blackRabbit.speak("Doom...");
// → The black rabbit says 'Doom...'

####prototype interference

A prototype can be used at any time to add new properties and methods to all objects based on it

####Prototype-less objects

Object.create function-allows us to create an object with a specific prototype. You are allowed to pass null through

####Polymorphism

any kind of object that supports this interface can be plugged into the code, and it will work

####tabel

minHeight() returns a number indicating the minimum height this cell requires (in lines).

minWidth() returns a number indicating this cell’s minimum width (in characters).

 draw(width, height) returns an array of length height, which contains a series of strings that are each width characters wide. This represents the content of the cell.

 function drawTable(rows) {
  var heights = rowHeights(rows);
  var widths = colWidths(rows);

  function drawLine(blocks, lineNo) {
    return blocks.map(function(block) {
      return block[lineNo];
    }).join(" ");
  }

  function drawRow(row, rowNum) {
    var blocks = row.map(function(cell, colNum) {
      return cell.draw(widths[colNum], heights[rowNum]);
    });
    return blocks[0].map(function(, lineNo) {
      return drawLine(blocks, lineNo);
    }).join("\n");
  }

  return rows.map(drawRow).join("\n");
}

####getters and setters

specify properties that look like normal properties but secretly have methods associated with them

####The instanceof operator

sees through inherited types.

 An RTextCell is an instance of TextCell because RTextCell.prototype derives from TextCell.prototype.

 The operator can be applied to standard constructors like Array. Almost every object is an instance of Object.
