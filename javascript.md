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

#Chapter 8

Bugs and Error Handling

bugs-flaws in a Program

####Programmer mistakes

-typos

Javascript doesnt help to find mistakes

Javascript catches errors that are not syntactically correct

most times it outputs a NaN or undefined values

debugging-process of finding mistakes

####Strict mode

if you use "use strict" at the top of file or function body

ex:

function canYouSpotTheProblem() {
  "use strict";
  for (counter = 0; counter < 10; counter++)
    console.log("Happy happy");
}

canYouSpotTheProblem();
// → ReferenceError: counter is not defined

forgetting var before defining a variable will give an error instead of using the global scope

this. value holds undefined function and registers error instead using global

wont allow a function to have more than one parameter of the same name

####Testing

you can write a second program in order to test your program

example program

function Vector(x, y) {
  this.x = x;
  this.y = y;
}
Vector.prototype.plus = function(other) {
  return new Vector(this.x + other.x, this.y + other.y);
};

testing program:

function testVector() {
  var p1 = new Vector(10, 20);
  var p2 = new Vector(-10, 5);
  var p3 = p1.plus(p2);

  if (p1.x !== 10) return "fail: x property";
  if (p1.y !== 20) return "fail: y property";
  if (p2.x !== -10) return "fail: negative x property";
  if (p3.x !== 0) return "fail: x from plus";
  if (p3.y !== 25) return "fail: y from plus";
  return "everything ok";
}
console.log(testVector());
// → everything ok

test suites:pieces of software that help you build and run collections of tests by providing a language (in the form of functions and methods) suited to expressing tests and by outputting info when a test fails. aka-testing frameworks.

####Debugging

sometimes itll point to line of error

think what is happening, why its happening and how to change it

use debugging tools in browsers

####Exceptions

exception handeling jumps back to where the program is working

set “obstacles” along the stack to catch the exception as it is zooming down. Then you can do something with it, after which the program continues running at the point where the exception was caught.

example

function promptDirection(question) {
  var result = prompt(question, "");
  if (result.toLowerCase() == "left") return "L";
  if (result.toLowerCase() == "right") return "R";
  throw new Error("Invalid direction: " + result);
}

function look() {
  if (promptDirection("Which way?") == "L")
    return "a house";
  else
    return "two angry bears";
}

try {
  console.log("You see", look());
} catch (error) {
  console.log("Something went wrong: " + error);
}

throw:raise exception

try{}catch{}-catching exception

  stack-trace

#Chapter 9

regular expressions-tool that describes patterns in string Data-read

type of object

var re1=new RegExp("string");
var re2=/string/;

if there is another slash you have to take into account

var eighteenPlus = /eighteen\+/;

####Testing for matches

If you pass it a string, it will return true/false telling you if the string contains a match of the pattern in the expression.

console.log(/abc/.test("abcde"));
// → true

if abc occurs anywhere in string it will return true

console.log(/abc/.test("abxde"));
// → false

####matching a set of characters

putting a set of numbers between square brackets makes that part of the expression match any of the characters between the brackets.

console.log(/[0123456789]/.test("in 1992"));
// → true
console.log(/[0-9]/.test("in 1992"));
// → true

\d means [0-9]

\w	An alphanumeric character (“word character”)

\s	Any whitespace character (space, tab, newline, and similar)

\D	A character that is not a digit

\W	A nonalphanumeric character

\S	A nonwhitespace character
.	Any character except for newline

var dateTime = /\d\d-\d\d-\d\d\d\d \d\d:\d\d/;

console.log(dateTime.test("30-01-2003 15:20"));

// → true

console.log(dateTime.test("30-jan-2003 15:20"));

// → false

var notBinary = /[^01]/;

to test for not 1s and 0s

####Repeating parts of a pattern

+ element may be repeated more than once

* allows the pattern to match 0 times

? makes it Optional

how many times a thing is supposed to happen

var dateTime = /\d{1,2}-\d{1,2}-\d{4} \d{1,2}:\d{2}/;

console.log(dateTime.test("30-1-2003 8:45"));
// → true

open digit range {4,}

####Grouping subexpressions

var cartoonCrying = /boo+(hoo+)+/i;
console.log(cartoonCrying.test("Boohoooohoohooo"));
// → true

i makes it case insensitive

####Matches and groups

execute methode-returns null if no match
and returns object with info if does match

var match = /\d+/.exec("one two 100");
console.log(match);
// → ["100"]
console.log(match.index);
// → 8

tells where the match started

####The Date type

to get current date and times

console.log(new Date());

function findDate(string) {
  var dateTime = /(\d{1,2})-(\d{1,2})-(\d{4})/;
  var match = dateTime.exec(string);
  return new Date(Number(match[3]),
                  Number(match[2]) - 1,
                  Number(match[1]));
}
console.log(findDate("30-1-2003"));
// → Thu Jan 30 2003 00:00:00 GMT+0100 (CET)

####Word and string boundaries

^start

$end

####choicepatterns

a number followed by one of the words pig, cow, or chicken, or any of their plural forms.

var animalCount = /\b\d+ (pig|cow|chicken)s?\b/;

console.log(animalCount.test("15 pigs"));
// → true

console.log(animalCount.test("15 pigchickens"));
// → false

####backtracking

/\b([01]+b|\d+|[\da-f]+h)\b/

binary,regular decimal,or hexadecimal

if one branch doesnt wor out, goes back to try the other ones, will stop at first full match

####the replace method

you can replace part of a string with another string

console.log("Borobudur".replace(/[ou]/, "a"));
// → Barobudur
console.log("Borobudur".replace(/[ou]/g, "a"));
// → Barabadar

by adding the g it replaces all os and us in the string with a

we can combine matching and replacing to swap placements like lastname, firstname to firstname lastname

console.log(
  "Hopper, Grace\n
  McCarthy, John\n
  Ritchie, Dennis"
    .replace(/([\w ]+), ([\w ]+)/g, "$2 $1"));
// → Grace Hopper
//   John McCarthy
//   Dennis Ritchie

$2 and $1 are parenthesized groups in the pattern up to $9 or all by $&

using functions to replace

var s = "the cia and fbi";
console.log(s.replace(/\b(fbi|cia)\b/g, function(str) {
  return str.toUpperCase();
}));
// → the CIA and FBI

or

var stock = "1 lemon, 2 cabbages, and 101 eggs";
function minusOne(match, amount, unit) {
  amount = Number(amount) - 1;
  if (amount == 1) // only one left, remove the 's'
    unit = unit.slice(0, unit.length - 1);
  else if (amount == 0)
    amount = "no";
  return amount + " " + unit;
}
console.log(stock.replace(/(\d+) (\w+)/g, minusOne));
// → no lemon, 1 cabbage, and 100 eggs

####The search method

shows where it was found or -1 if it wasnt

console.log("  word".search(/\S/));
// → 2

console.log("    ".search(/\S/));
// → -1

####The lastIndex property

source-string expression was created from

lastindex-where next match will start

####Looping over matches

var input = "A string with 3 numbers in it... 42 and 88.";
var number = /\b(\d+)\b/g;
var match;
while (match = number.exec(input))
  console.log("Found", match[1], "at", match.index);
// → Found 3 at 14
//   Found 42 at 33
//   Found 88 at 40

####Parsing an INI file

Blank lines and lines starting with semicolons are ignored.

Lines wrapped in [ and ] start a new section.

Lines containing an alphanumeric identifier followed by an = character add a setting to the current section.

Anything else is invalid.

split method also allows a regular expression as its argument, we can split on a regular expression like /\r?\n/ to split in a way that allows both "\n" and "\r\n" between lines.
});

####RegExp

/abc/	A sequence of characters

/[abc]/	Any character from a set of characters

/[^abc]/	Any character not in a set of characters

/[0-9]/	Any character in a range of characters

/x+/	One or more occurrences of the pattern x

/x+?/	One or more occurrences, nongreedy

/x*/	Zero or more occurrences

/x?/	Zero or one occurrence

/x{2,4}/	Between two and four occurrences

/(abc)/	A group

/a|b|c/	Any one of several patterns

/\d/	Any digit character

/\w/	An alphanumeric character (“word character”)

/\s/	Any whitespace character

/./	Any character except newlines

/\b/	A word boundary

/^/	Start of input

/$/	End of input

###extra notes

reg expresions-a pattern that a string can match

^\d{5}(\-\d{4})?$

01331-3859

^ beginning first digit must be a number and there must be 5 numbers in a row the ? means entire group is optional and $ means its the end no extra between big and end

#Chapter 10

like chapters and sections in a book

why use modules:

maintainability: self-contained.

namespacing:sharing global variables between unrelated code is not okay

reusability:instead of updating everypiece of code you can reuse modules

decoupling:isolates code from eachother

allows module to grow

####Using Functions as namespacing

var dayName = function() {
  var names = ["Sunday", "Monday", "Tuesday", "Wednesday",
               "Thursday", "Friday", "Saturday"];
  return function(number) {
    return names[number];
  };
}();

console.log(dayName(3));
// → Wednesday

define variables inside of functions to keep them outside of global scope

####Objects as interfaces

in order to return function you have to wrap two functions inside an Object

var weekDay = function() {
  var names = ["Sunday", "Monday", "Tuesday", "Wednesday",
               "Thursday", "Friday", "Saturday"];
  return {
    name: function(number) { return names[number]; },
    number: function(name) { return names.indexOf(name); }
  };
}();

console.log(weekDay.name(weekDay.number("Sunday")));
// → Sunday

(function(exports) {
  var names = ["Sunday", "Monday", "Tuesday", "Wednesday",
               "Thursday", "Friday", "Saturday"];

  exports.name = function(number) {
    return names[number];
  };
  exports.number = function(name) {
    return names.indexOf(name);
  };
})(this.weekDay = {});

console.log(weekDay.name(weekDay.number("Saturday")));
// → Saturday

module function takes its interface object as an argument, allowing code outside of the function to create it and store it in a variable.

####Detaching from the global scope

create a system that allows one module to directly ask for the interface object of another module, without going through the global scope

require function that will load that module’s file (from disk or the Web, depending on the platform we are running on) and return the appropriate interface value.

need two things

1:readFile function that returns content as a string

2:execute string as javascript

####Evaluating data as code

eval-excecutes a string in the current scope

use Function Constructor two arguments

var plusOne = new Function("n", "return n + 1;");
console.log(plusOne(4));
// → 5

####require

function require(name) {
  var code = new Function("exports", readFile(name));
  var exports = {};
  code(exports);
  return exports;
}

console.log(require("weekDay").name(1));
// → Monday

var names = ["Sunday", "Monday", "Tuesday", "Wednesday",
             "Thursday", "Friday", "Saturday"];

exports.name = function(number) {
  return names[number];
};
exports.number = function(name) {
  return names.indexOf(name);
};

var weekDay = require("weekDay");
var today = require("today");

console.log(weekDay.name(today.dayNumber()));

better:

function require(name) {
  if (name in require.cache)
    return require.cache[name];

  var code = new Function("exports, module", readFile(name));
  var exports = {}, module = {exports: exports};
  code(exports, module);

  require.cache[name] = module.exports;
  return module.exports;
}
require.cache = Object.create(null);

commonjsmodules

####Interface Design

predictabiity-follow conventions so other programmers can help

the actual behavior of it

####composability
try using pure functions

module needs to be able to compose easily with other

####Layered interfaces

provide two interfaces a low and high level

#chapter12

url- uniform resourcw locator

http://-protocol

eloquentjavastcript.net/-server

12_browser.html-path

every computer has unique ip bbut are substituted with domain names

html is the way the document is formatted

script allows us to acces javascfipt in our html documents

sandboxing-isolating a programs environment

#chapter13

document- lets us access objects
and documentElement is the object of the html tangent

####trees

datastructures are called trees ifit has branches

trees have different kind of nodes

html -head and body

head-title-"words"

body-h1,p-"words"/links

####Moving through the tree

function talksAbout(node, string) {
  if (node.nodeType == document.ELEMENT_NODE) {
    for (var i = 0; i < node.childNodes.length; i++) {
      if (talksAbout(node.childNodes[i], string))
        return true;
    }
    return false;
  } else if (node.nodeType == document.TEXT_NODE) {
    return node.nodeValue.indexOf(string) > -1;
  }
}

console.log(talksAbout(document.body, "book"));
// → true

getElementsByTagName method, which collects all elements with the given tag name

getElementById

getAttribute and setAttribute methods

class

offsetWidth offsetHeight -space the element takes up in pixels

clientWidth and clientHeight-size of the space inside element

getBoundingClientRect method. It returns an object with top, bottom, left, and right properties, indicating the pixel positions of the sides of the element relative to the top left of the screen

querySelectorAll- takes a selector string and returns an array-like object containing all the elements that it matches.

#chapter14

<p>Click this document to activate the handler.</p>
<script>
  addEventListener("click", function() {
    console.log("You clicked!");
  });
</script>

"click"

addEventListener has two arguments the second being a function that logs something to the console when it is clicked

to prevent default mehtods associated with handlers use prevetnDefault on the object

/*<a href="https://developer.mozilla.org/">MDN</a>/*
<script>
  var link = document.querySelector("a");
  link.addEventListener("click", function(event) {
    console.log("Nope.");
    event.preventDefault();
  });
</script>

when key is pressed=keydown

not-keyup

console.log("Violet".charCodeAt(0));
// → 86
console.log("1".charCodeAt(0));
// → 49

to find numeric code of letter wanting to have event

keypress is the text

mouesdown, mouse up, click,dblclick,mousemove, mouseout,

use relatedTarget

isInside

scroll

focus

onchange-An HTML element has been changed

onclick-The user clicks an HTML element

onmouseover-The user moves the mouse over an HTML element

onmouseout-The user moves the mouse away from an HTML element

onkeydown-The user pushes a keyboard key

onload-The browser has finished loading the page

#chapter17

####http

hyper transfer protocol-how data is requested and provided on the Web

steps to find this link

eloquentjavascript.net/17_http.html

1-(request)looks up the address of the server associated with eloquentjavascript.net and tries to open a TCP connection to it on port 80, the default port for HTTP

browser sends something like this:

GET /17_http.html HTTP/1.1

---(GET is the method(DELETE,PUT to replace, POST to send))

---(HTTP/1.1  version HTTP)

Host: eloquentjavascript.net

---(path of the resource)

User-Agent: Your browser's name

2-server responds

HTTP/1.1 200 OK

---(version and status of response, in numbers then human language)

------code start with 2-code suceeded

------code start with 4- error on request(404)

------code start with 5-server error

---the rest are exra headers

Content-Length: 65585

---size if document in bytes

Content-Type: text/html

---type of document

Last-Modified: Wed, 09 Apr 2014 10:48:09 GMT

---when it was last modified

<!doctype html> (start of document)

... the rest of the document

####Browsers and HTTP

#####GET

handle multiple request simultaniously using GET request

forms can be filled out and sent back to the server

<form method="GET" action="example/message.html">

  <p>Name: <input type="text" name="name"></p>

  <p>Message:<br><textarea name="message"></textarea></p>

  <p><button type="submit">Send</button></p>

</form>

when you click the Send button, the information in those fields will be encoded into a query string.

When the <form> element’s method attribute is GET (or is omitted), that query string is tacked onto the action URL, and the browser makes a GET request to that URL.

GET /example/message.html?name=Jean&message=Yes%3F HTTP/1.1

?-start of a query string

pairs of names and values, corresponding to the name attribute on the form field elements and the content of those elements, respectively. An ampersand character (&) is used to separate the pairs.

name=Jean&message=Yes?

the question mark in the message must be escaped so it has % and its character code in hexadecimal

encodeURIComponent and decodeURIComponent functions-encode and decode this format.

console.log(encodeURIComponent("Hello & goodbye"));
// → Hello%20%26%20goodbye
console.log(decodeURIComponent("Hello%20%26%20goodbye"));
// → Hello & goodbye

#####POST

POST /example/message.html HTTP/1.1

Content-length: 24

Content-type: application/x-www-form-urlencoded

name=Jean&message=Yes%3F

put the query string in body of the request, rather than adding it to the URL.

GET method is used for requests that do not have side effects, such as doing a search

POST-Requests that change something on the server, such as creating a new account or posting a message

####XMLHttpRequest

interface through which browser JavaScript can make HTTP requests

####Sending a request

to make a simple request-create a request object with the XMLHttpRequest constructor and call its open and send methods.

var req = new XMLHttpRequest();

req.open("GET", "example/data.txt", false);

---( open method configures the request )

req.send(null);

console.log(req.responseText);

// → This is the content of data.txt

console.log(req.status, req.statusText);

// → 200 OK

console.log(req.getResponseHeader("content-type"));

// → text/plain

If we pass true as the third argument to open, the request is asynchronous. This means that when we call send, the only thing that happens right away is that the request is scheduled to be sent. Our program can continue, and the browser will take care of the sending and receiving of data in the background.

as the request is running, we won’t be able to access the response unless we use load


var req = new XMLHttpRequest();

req.open("GET", "example/data.txt", true);

req.addEventListener("load", function() {

  console.log("Done:", req.status);

  ---(a mechanism that will notify us when the data is available.)

});

req.send(null);

####Fetching XML Data

resource retrieved by an XMLHttpRequest object is an XML document, the object’s responseXML property will hold a parsed representation of this document.

 The object that responseXML holds corresponds to the document object. Its documentElement property refers to the outer tag of the XML document. In the following document (example/fruit.xml), that would be the <fruits> tag:

<fruits>
  <fruit name="banana" color="yellow"/>
  <fruit name="lemon" color="yellow"/>
  <fruit name="cherry" color="red"/>
</fruits>


var req = new XMLHttpRequest();

req.open("GET", "example/fruit.xml", false);

req.send(null);

console.log(req.responseXML.querySelectorAll("fruit").length);
// → 3

better idea to communicate using JSON data

var req = new XMLHttpRequest();
req.open("GET", "example/fruit.json", false);
req.send(null);
console.log(JSON.parse(req.responseText));
// → {banana: "yellow", lemon: "yellow", cherry: "red"}


Access-Control-Allow-Origin: *

servers can include a header in their response to indicate that it is okay for the request to come from other domains:

#####Abstracting request

function backgroundReadFile(url, callback) {

  var req = new XMLHttpRequest();

  req.open("GET", url, true);

  req.addEventListener("load", function() {

    if (req.status < 400)

      callback(req.responseText);

  });

  req.send(null);

}

the function makes it easier to use XMLHttpRequest for simple GET requests

Tip:good idea to use a helper function so that you don’t end up repeating XMLHttpRequest pattern all through your code.

---callback function is given to other code to provide that code with a way to “call us back” later.

^only supports GET

problem: handling of failure

--request returns a status code thats an error (400+), it does nothing

--if put a “loading” indicator on the page to indicate that we are fetching information

--if request fails the page will sit there

option to be notified when the request fails so that we can take appropriate action

function getURL(url, callback) {
  var req = new XMLHttpRequest();
  req.open("GET", url, true);
  req.addEventListener("load", function() {
    if (req.status < 400)
      callback(req.responseText);
    else
      callback(null, new Error("Request failed: " +
                               req.statusText));
  });
  req.addEventListener("error", function() {
    callback(null, new Error("Network error"));
  });
  req.send(null);
}

Code using getURL must then check whether an error was given and, if it finds one, handle it

getURL("data/nonsense.txt", function(content, error) {

  if (error != null)

    console.log("Failed to fetch nonsense.txt: " + error);

  else

    console.log("nonsense.txt: " + content);

});

####Promises

Promises wrap an asynchronous action in an object, which can be passed around and told to do certain things when the action finishes or fails

promise object:

---call the Promise constructor and give it a function that initializes the asynchronous action

---he constructor calls that function, passing it two arguments, which are themselves functions

---The first should be called when the action finishes successfully, and the second should be called when it fails.

function get(url) {

  return new Promise(function(succeed, fail) {

    var req = new XMLHttpRequest();

    req.open("GET", url, true);

    req.addEventListener("load", function() {

      if (req.status < 400)

        succeed(req.responseText);

      else

        fail(new Error("Request failed: " + req.statusText));

    });

    req.addEventListener("error", function() {

      fail(new Error("Network error"));

    });

    req.send(null);

  });

}

Calling then produces a new promise

####Security and https

secure HTTP protocol-https:// wraps HTTP traffic in a way that makes it harder to read and tamper with

#chapter 18

####fields

different styles-simple on/off checkboxes to drop-down menus and fields for text input.

text	A single-line text field

password	Same as text but hides the text that is typed

checkbox	An on/off switch

radio	(Part of) a multiple-choice field

file	Allows the user to choose a file from their computer

fields can not be submitted only forms can

<p><input type="text" value="abc"> (text)</p>

<p><input type="password" value="abc"> (password)</p>

<p><input type="checkbox" checked> (checkbox)</p>

<p><input type="radio" value="A" name="choice">
   <input type="radio" value="B" name="choice" checked>
   <input type="radio" value="C" name="choice"> (radio)</p>

<p><input type="file"> (file)</p>

Multiline text fields have their own tag, <textarea></textarea>

<select> tag is used to create a field that allows the user to select from a number of predefined options.

<select>
  <option>Pancakes</option>
  <option>Pudding</option>
  <option>Ice cream</option>
</select>

"change"event-when value of form field changes

####focus

form fields can get keyboard focus

---when clicked or activated they re a currently active element and the key board is focused to them

focus: moves focus to the DOM element it is called on

blur:removes focus

document.activeElement is the focused element.

<input type="text">

<script>

  document.querySelector("input").focus();

  console.log(document.activeElement.tagName);

  // → INPUT

  document.querySelector("input").blur();

  console.log(document.activeElement.tagName);

  // → BODY

</script>

users can tab through fields, create that order by using

<input type="text" tabindex=1> <a href=".">(help)</a>

<button onclick="console.log('ok')" tabindex=2>OK</button>

####Disabled fields

all fields can be Disabled

<button>I'm all right</button>
<button disabled>I'm out</button>

prevents user when clicking not to redo actions

####forms

The <form> element, in turn, has a property called elements that contains an array-like collection of the fields inside it.

ways to acccess:

 array-like object (accessible by number)

  and a map (accessible by name).

####Text Fields

Input Tags

--text

--password

--textarea

value of DOM elements is the current content as a string

setting property to another string changes the value to that string

selectionStart & selectionEnd

--give us information about the cursor and selection in the text

when nothing is selected both are equal

example:

if i have sected from the beginning of text to 10nth character it will be 0 for start and 20 for end

replaceSelection

--replaces the currently selected part of a text field’s content

shows current length of text

<input type="text"> length: <span id="length">0</span>

<script>

  var text = document.querySelector("input");

  var output = document.querySelector("#length");

  text.addEventListener("input", function() {

    output.textContent = text.value.length;

  });

</script>

 changes everytime a types a character, deletes text, or otherwise manipulates the field’s content rather than when focused and unfocused

####Checkboxes and radio buttons

changes color of page to purple when clicked

<input type="checkbox" id="purple">

<label for="purple">Make this page purple</label>

<script>

  var checkbox = document.querySelector("#purple");

  checkbox.addEventListener("change", function() {

    document.body.style.background =

      checkbox.checked ? "mediumpurple" : "";

  });

</script>

<label> is used to associate a piece of text with an input field.

Its for attribute should refer to the id of the field.

Clicking the label will activate the field, which focuses it and toggles its value when it is a checkbox or radio button.

radio button-linked to other radio buttons with the same name attribute so that only one of them can be active at any time.


Color:


<input type="radio" name="color" value="mediumpurple"> Purple

<input type="radio" name="color" value="lightgreen"> Green

<input type="radio" name="color" value="lightblue"> Blue

<script>

  var buttons = document.getElementsByName("color");

  function setColor(event) {

    document.body.style.background = event.target.value;

  }

  for (var i = 0; i < buttons.length; i++)

    buttons[i].addEventListener("change", setColor);

</script>

--document.getElementsByName - all elements with a given name attribute

####Select fields

appearance is determined by the browser

When given the multiple attribute, will allow the user to select any number of options, rather than just a single option

--choose all that apply

<select multiple>

  <option>Pancakes</option>

  <option>Pudding</option>

  <option>Ice cream</option>

</select>

--size attribute:  used to set the number of options that are visible at the same time

setting the size attribute to "3" will make the field show three lines, whether it has the multiple option enabled or not

value property of a <select> element reflects the currently selected option

a multiple field this property will give the value of only one of the currently selected options

options property- accessed as an array-like object

--selected- indicates whether that option is currently selected. can over ride selected or deselection here

####file fields

a way to upload files from the browser’s machine through a form

provide a way to read such files from JavaScript programs

acts as a gatekeeper

browse is the most known example of this

<input type="file">

<script>

  var input = document.querySelector("input");

  input.addEventListener("change", function() {

    if (input.files.length > 0) {

      var file = input.files[0];

      console.log("You chose", file.name);

      if (file.type)

        console.log("It has type", file.type);

    }

  });

</script>

--files - rray-like object containing the files chosen in the field.

 initially empty.

  also support a multiple attribute

  Objects in the files property:

  --- name (the filename)

  ---size (the file’s size in bytes)

  ---type (the media type of the file, such as text/plain or image/jpeg).

!!!does not have is a property that contains the content of the file.!!!

FileReader constructor as being similar to XMLHttpRequest but for files.

<input type="file" multiple>

<script>

  var input = document.querySelector("input");

  input.addEventListener("change", function() {

    Array.prototype.forEach.call(input.files, function(file) {

      var reader = new FileReader();

      reader.addEventListener("load", function() {

        console.log("File", file.name, "starts with",

                    reader.result.slice(0, 20));

      });

      reader.readAsText(file);

    });

  });

</script>

explanation: Reading a file is done by creating a FileReader object, registering a "load" event handler for it, and calling its readAsText method, giving it the file we want to read. Once loading finishes, the reader’s result property contains the file’s content.

can wrap in promise:

function readFile(file) {

  return new Promise(function(succeed, fail) {

    var reader = new FileReader();

    reader.addEventListener("load", function() {

      succeed(reader.result);

    });

    reader.addEventListener("error", function() {

      fail(reader.error);

    });

    reader.readAsText(file);

  });

}

####Storing data client-side

Sometimes it is enough to just keep the data in the browser. But how?

localStorage object: store string data to not reload


localStorage.setItem("username", "marijn");

console.log(localStorage.getItem("username"));

// → marijn

localStorage.removeItem("username");

localStorage sticks around until it is overwritten, it is removed with removeItem, or the user clears their local data.

Notes: <select id="list"></select>
<button onclick="addNote()">new</button><br>
<textarea id="currentnote" style="width: 100%; height: 10em">
</textarea>

<script>
  var list = document.querySelector("#list");
  function addToList(name) {
    var option = document.createElement("option");
    option.textContent = name;
    list.appendChild(option);
  }

  // Initialize the list from localStorage
  var notes = JSON.parse(localStorage.getItem("notes")) ||
              {"shopping list": ""};
  for (var name in notes)
    if (notes.hasOwnProperty(name))
      addToList(name);

  function saveToStorage() {
    localStorage.setItem("notes", JSON.stringify(notes));
  }

  var current = document.querySelector("#currentnote");
  current.value = notes[list.value];

  list.addEventListener("change", function() {
    current.value = notes[list.value];
  });
  current.addEventListener("change", function() {
    notes[list.value] = current.value;
    saveToStorage();
  });

  function addNote() {
    var name = prompt("Note name", "");
    if (!name) return;
    if (!notes.hasOwnProperty(name)) {
      notes[name] = "";
      addToList(name);
      saveToStorage();
    }
    list.value = name;
    current.value = notes[name];
  }
</script>

a simple note-taking application.

It keeps the user’s notes as an object, associating note titles with content strings.

This object is encoded as JSON and stored in localStorage. The user can select a note from a <select> field and change that note’s text in a <textarea>.

 A note can be added by clicking a button.

sessionStorage-content of sessionStorage is forgotten at the end of each session, which for most browsers means whenever the browser is closed.

#Scopes and closures

####Scope:

where  variables are stored and how to find them

####Compiler theory

3 steps:

1)Tokenizing/Lexing:

2)Parsing:

3)Code-Generation:

####Conversation

the cast:

Engine: responsible for start-to-finish of JavaScript

Compiler: one of Engine's friends; handles all the dirty work of parsing and code-generation

Scope: another friend of Engine; collects and maintains a look-up list of all the declared identifiers (variables), and enforces a strict set of rules as to how these are accessible to currently executing code.

back and forth:

var a =2;

engine sees 2 parts: complier will handle one and engine the other

complier-prwforms Lexing tobreak down tokens var,a,=,2,; then parse into a tree but when it comes to code generation it will:

encounter var a it ask scope if a already exist if so it ignores the var a part if not it declares a new variabe called a

produces code a = 2 if a already exist it will replace a value with 2

First, Compiler declares a variable (if not previously declared in the current scope), and second, when executing, Engine looks up the variable in Scope and assigns to it, if found.

####compiler speak

LHS RHS left hand side and right hand side of an assignment operation

lhs looks for the container the value is stored in

rhs anything other than container

console.log( a );

The reference to a is an RHS reference, because nothing is being assigned to a here. Instead, we're looking-up to retrieve the value of a, so that the value can be passed to console.log(..).

a = 2;

LHS reference, because we don't actually care what the current value is, we simply want to find the variable as a target for the = 2

####Engine/scope Conversation

Engine: Hey Scope, I have an RHS reference for foo. Ever heard of it?

Scope: Why yes, I have. Compiler declared it just a second ago. He's a function. Here you go.

Engine: Great, thanks! OK, I'm executing foo.

Engine: Hey, Scope, I've got an LHS reference for a, ever heard of it?

Scope: Why yes, I have. Compiler declared it as a formal parameter to foo just recently. Here you go.

Engine: Helpful as always, Scope. Thanks again. Now, time to assign 2 to a.

Engine: Hey, Scope, sorry to bother you again. I need an RHS look-up for console. Ever heard of it?

Scope: No problem, Engine, this is what I do all day. Yes, I've got console. He's built-in. Here ya go.

Engine: Perfect. Looking up log(..). OK, great, it's a function.

Engine: Yo, Scope. Can you help me out with an RHS reference to a. I think I remember it, but just want to double-check.

Scope: You're right, Engine. Same guy, hasn't changed. Here ya go.

Engine: Cool. Passing the value of a, which is 2, into log(..).

####Nested scopes

usually more than one Scope  to consider

Engine: "Hey, Scope of foo, ever heard of b? Got an RHS reference for it."

Scope: "Nope, never heard of it. Go fish."

Engine: "Hey, Scope outside of foo, oh you're the global Scope, ok cool. Ever heard of b? Got an RHS reference for it."

Scope: "Yep, sure have. Here ya go."

engine starts at the currently executing Scope, looks for the variable there, then if not found, keeps going up one level

tall building enter front door

####errors:

two types of look-ups behave differently in the circumstance where the variable has not yet been declared

####Lexical scope

"scope" as the set of rules that govern how the Engine can look up a variable by its identifier name and find it

lexing process examines a string of source code characters and assigns semantic meaning to the tokens as a result of some stateful parsing

lexical scope is based on where variables and blocks of scope are authored, by you, at write time, and thus is (mostly) set in stone by the time the lexer processes your code.

scopes are bubbles inside eachother

####Lookups

Scope look-up stops once it finds the first match

Scope look-up stops once it finds the first match

eval(..) function in JavaScript takes a string as an argument, and treats the contents of the string as if it had

 actually been authored code at that point in the program

 allows you to modify the lexical scope environment by cheating and pretending that author-time

 with is typically explained as a short-hand for making multiple property references against an object without repeating the object reference itself each time.

####Function vs block scope

scope consists of a series of "bubbles" that each act as a container or bucket, in which identifiers (variables, functions) are declared.

 These bubbles nest neatly inside each other, and this nesting is defined at author-time.

 what makes a new bubble? Is it only the function? Can other structures in JavaScript create bubbles of scope?

#####scope from functions

function foo(a) {
    var b = 2;

    // some code

    function bar() {
        // ...
    }

    // more code

    var c = 3;
}

scope: a, b, c and bar

not accessible outside of foo(..)

each function you declare creates a bubble for itself, but no other structures create their own scope bubbles

!!!!you declare a function, and then add code inside it
