#CSS3 Notes

compatibility of html5

 &lt;!--[if lt IE 9]&gt;

 &lt;script src="//html5shiv.googlecode.com/
    svn/trunk/html5.js"&gt;&lt;/script&gt;
    &lt;![endif]--&gt;

make sure IE is up to date

###CSS creating styles and style sheet

how to format the pages

selctor {
  property:value
}

internal and external css

* universal selector
\

###Adding graphics to webpage

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

###Tables and forms

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

**Preventing float drops

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

*media queries:

adjust columns

flexile widths

tighten up white space

adjusting font sizes

change navigation menus

hide content on mobile devices

*breakpoint at which point do things change

smartphones, tablets, and desktop monitors

start with default design then create media querie syles to override default styles and to reformat the pages

*main approaches

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

      @import url(css/base.css); no media query, applies to all */

     @import url(css/medium.css) (min-width:481px) and (max-width:768);

     @import url(css/small.css) (max-width: 480px);

*flexible grids use percentages

box-sizing:border box to git rid of float drops

*Fluid Images:

img{
  max-width:100%
}
