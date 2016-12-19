#CSS3 Notes

###Chapter1

compatibility of html5

 &lt;!--[if lt IE 9]&gt;

 &lt;script src="//html5shiv.googlecode.com/
    svn/trunk/html5.js"&gt;&lt;/script&gt;
    &lt;![endif]--&gt;

make sure IE is up to date

###Chapter2

CSS creating styles and style sheet

how to format the pages

selector-tells browser which elements to style.

declaration block-where you put all of the styles

declarations-thestyles themselves

properties- what youre changing

value-how youre changing the property

internal use style in head section followed by the CSS

external use link in head to separate page where css is

###Chapter3

selctor {
  property:value
}

internal and external css

* universal selector

ancestor

descndent

parent

child

sibling

pseudo classes/elements

classes:

a:link

a:visited

a:hover

a:active

a:focus

:first-letter,first-line

elements:

before:adds content preceding any element

after:adds content after elements

::selection

Child:

:first-child :lastchild, nth-child

:first of type lastof type
nth of type

Siblings

:not()

###Chapter4

Style inheritance

 properties that affect the placement of elements on the page or the margins, background colors, and borders of elements aren’t inherited.

###Chapter5

Managing multiple style sheets

nearest ancestor wins

direct applied style wins

inline style id then class tag

last style breaks the tie

avoiding specificity ward

###Chapter6

Formatting text

fonts:only certain fonts are supported on different browsers

serif-long passages

sans serif- headlines

web fonts @font face

EOT:embedded open type

true type and open type

web open font format

scalable vector graphics

*legal isues*

font size

px,ems,%

italicizing and bolding

font-variant:small caps

text-decorating

underline,overline ect

letter and word text shadow

space between lines, indents,first letter, lines

styling list

list-style-position (outside or inside)

graphic bullets

###Chapter 7

Margins padding and borders

Box Model:

content-padding(space between content and border)-border(around padding and content)-margin(around element)

you can use magins and padding to layout an entire page

TRBL-TRouBLE

use negative margins to remove space

inline-follows previous element, block-creates break after

add borders for design

size,style,and color

rounded corners

border-radius

drop shadows-make it popo on the page

### Chapter 8 Adding graphics to webpage

borders-around an image

padding-space between border and image

float-move to left or right edge of page

margins-space between image and other content

####background-image

background-image:url();

controlling repetition

background-repeat:no-repeat;

displays image single times

repeat-x

repeats image horizontally

repeat-y

repeats vertically

positioning background-image

background-position:

center center

right top

center top

px px

% %

em em

background attachment: fixed

keeps background from scrolling with pages

defining orgin and clipping

border-box places the image in the upper-left corner of the area assigned to the border

padding-box places the image in the upper-left corner of the area assigned to the padding  This is normally where a browser places a background image.

content-box places the image in the upper-right corner of the area assigned to the content

background-size: 100% 100%

contain maintains ratio while resizing image

link status: particular order: link, visited, hover, and active.

###Chapter 9

Navigation Bar

LoVe/HAte

using graphics

padding allows room

psuedo classes add helpful feedback

use unordered list for nav bars

remove bullets and get rid of padding

Vertical nav bars: use blocks,liit the width

horizontal nav bars:inline-block

Preloading rollovers:

style links

###Chapter 10 Animations

####transform:

rotate- degree from 0-360

scale-resize an element

 translate-moves an element left right up and down

skew: simulates 3d look distorts element by using degrees

multiple:      transform: skew(45deg,0deg) scale(.5) translate(400px,500px) rotate(90deg);

order is based on order of elements

change orgin from center:     

transform-origin: left top;

####transitions

two styles, before and after

apply to original styles

Trigger: action that causes the change

psuedo classes

:hover

:active

:target

:focus

transition-property:specifies what is being animated

transition-duration:how long animation takes to complete

transition-timing-function: speed of animation

linear,ease,ease-in,ease-out,and ease-in-out

transition:delay stop animation from occuring instantly

###Animations

1.Define animation

2.apply animation to an element

@keyframes name{
  from{

opacity:0;

  }

  to{

opacity:1;

  }

  }

}

shorthand

element{
  name, duration, timing function, count, direction, delay, and fill- mode
}

animation-play-state:running or paused

###chapter 11 Tables and forms

padding: top, right, bottom, left;

aligning text horizontially

table{
  text.align:left, right, center, justified;

  vertical-align:top, baseline, middle, bottom;
}

styling rows and colors

tr:nth-of-type(odd) { background-color: red; } tr:nth-of-type(even) { background-color: blue; }

styling forms

&lt;fieldset&gt; groups related form questions

&lt;legend&gt; provides label for group

###CSS layout

fixed-width- workswith having most control but doesnt allow

 visitors to resize pages

liquid- adjust to fit browsers width

Responsive web design uses media queries to send different designs to different width browsers

###Chapter 12

CSS layout

fixed-960px

liquid-adjust to fit browsers width

rwd-changes presentation per width

mobile first

identify boxes

go with flow

background images

layer elements accordingly

use margin and paddings


###chapter 13

position elements side by side  or a block

properties: left right and none

*2 column design:

put each column in div, float 1 to either side, set width, add margin to other column.

for more columns wrap every thing inside of one div

*3 columns follow steps for 2 but add another div between the

 two columns and float it right, add right margin

 *floating every column lets you put more than 3 columns in,

  manditory for the widths to add up or be less than main divs

   width.

Float problems:

clear:left, right or both

keeps content from wrapping around floats and stays under it

*full column heights

add a linear gradient with color stops at the widths of columns

background-image:linear-gradient(
  left,red 05, red 25%, white 25%,white 75%, blue 75%,blue 100%;)
  )

**Preventing float drops**

do the math include padding

use percentages and pad elements inside column

use box sizing

:content-box: normal browsers

:padding-box: include left and right padding

:border-box: includes padding borders and css width

###chapter 14

Responsive Web design

lets you build a single site that adapts to different device widths

3 main ideas:

grids for layouts-forger fixed widths

flexible media images-images scale to fit device screen

css media queries-send different styles based on conditions(width and height)

**    <meta name="viewport" content="width=device-width">

above title tag.

*media queries:*

adjust columns

flexile widths

tighten up white space

adjusting font sizes

change navigation menus

hide content on mobile devices

*breakpoint at which point do things change*

smartphones, tablets, and desktop monitors

start with default design then create media querie syles to override default styles and to reformat the pages

*main approaches*

Desktop first:do everything concerning desktop first then add media queries for phones/tablets

benifit is that browsers that dont understand it will get the desktop version

take away from this design

Mobile: youll add to this design

A querie is like asking a browser a yes or no question regarding the width and then browser launches styl

 sheet for that device

      <link href="css/small.css" rel="stylesheet" media="(width: 480px)">

media attribute sets the condition for the browsers

use max-width in media attribute to say anything under this width gets this style sheet

and a min width to say if its wider than this width

use both to set a range <link href="css/medium.css" rel="stylesheet" media="(min-width:481px) and
     (max-width:768px)">

     you can have one style sheet linking to all style sheets

      @import url(css/base.css); no media query, applies to all */*

     @import url(css/medium.css) (min-width:481px) and (max-width:768);

     @import url(css/small.css) (max-width: 480px);

*flexible grids use percentages*

box-sizing:border box to git rid of float drops

*Fluid Images:*

img{
  max-width:100%
}

###Chapter 15

Positioning elements on a web page

*Absolute positioning*

specific location completly detached from flow of elements

*relative positioning*

leaves hole in flow of page

*fixed*

locked into place on screen

*static*

normal top down flow

positioning has four properties

top

left

bottom

right

   A tag is positioned relative to the browser window if it has an absolute posi- tion and it’s not inside
  any other tag that has either absolute, relative, or fixed positioning applied to it.

   A tag is positioned relative to the edges of another element if it’s inside another tag with absolute, relative, or fixed positioning.

   z-index represents the order in which positioned elements are stacked on top of the page.

   *visibility*

   *opacity*

###Chapter 16

   CSS for the printed page

   printer friendly versions

   *Media Style Sheets*

   10 types

   all, braille, embossed, handheld, print, projection, screen, speech, tty, and tv.

   all-everydevice

   screen-display only on monitors

   print-apply only when the page is printed

   Adding media style Sheets

  HTML      <link rel="stylesheet" media="print" href="print.css"/>

  CSS @media print {

       /* put your styles for the printer in here */*

     }

     use pt when editing font size for print version 12 pt;

     page-break-before and page-break-after

###Chapter 17

Adding comments

/* comment(/**)

Name Style Clearly

by purpose, not appearance or position

Use multiple classes

Use comments to seperate
