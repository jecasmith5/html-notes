# HTML & CSS Notes

## Chapter One
### What is HTML
Describes the Structure of web pages

Hypertext markup language

### Tags

* &lt;doctype&gt;: version of html

&lt;html&gt;:whole page html code

&lt;head&gt;: information about the page, title & links

&lt;title&gt;:top of browser above url

&lt;body&gt;:shown inside main browser

&lt;meta&gt;:

do not effect display

define key words for search engines

author of  a page

refresh document...ect



### Structure
Headings and subheadings help to organize information

### Elements
opening &lt; &gt;

h1 main heading

p paragraph/ body of text

h2 subheading ect ..

closing &lt;/ &gt;

character inside brackets indicates purpose

### Attributes

Provide more information about whats inside the Elements

name and value seperated by equal sign

example: &lt;p lang="en-us"&gt;

name=lang    value="en-us"

### PC

START-
ALL PROGRAMS-
ACCESSORIES-
NOTEPAD-

NOTEPAD++ - FREE EDITOR

SAVE AS .html

### MAC
APPLICATIONS-TextEdit

TextWrangler - editor for creating web pages

file-
save as-
.html-
use.html-

### Content Management System

template to control each section

## Chapter Two
### Text
Structual markup- elements for headings and paragraphs

Semantic-extra information i.e emhasis in sentence, quotes, acronyms

#### Headings

*h1

*h2

*h3

*h4

*h5

*h6

text decreases throughout levels

css is in charge of fonts color and text size

#### Features

b - bold text enclose word or word with b in angle brackets

i - italic text i in angle brackets surrounding word or words

sup-supertext raising a number to a power or the 4th

sub- subscript footnotes or chemistry such as H20

auto collapsing white space

br / -adds break in middle of paragraph

hr / -horizontal line in between sections

break and horizontal line have no closing Tags

#### Visual editors

two views:
visual editor and code view

Visual is like word where you can see  what youre doing as in highlighting, bold, italics, ect.

code views show the code where you would manually edit such things

### Semantic markup

strong - strong importance bolds wording

em - emphasis in italics

blockquote -  quotes that take up entire paragraph

q -quotes within a paragraph

abbr - abbr title

cite - indicates where cite is from

dfn defining instance of a word

address- contact details for author of page

ins - underlines

del- crossed out

s- no longer relevant, prices line through center

### Chapter 3

ol - ordered list use numbers

1.

2.

3.

li - inside ol opening and closing per item in list

ul - unordered list use bullets

*

*

*

li - use inside ul

dl - definition list

dt - term being defined

hello

dd - definition of term

greeting

nested list create list inside of list

###Chapter 4

### links

a element, able to click on anything between open and closing of a


example

&lt;a href="http://www.imbd.com"&gt;IMBD&lt;/a &gt;


#### links to different website, use absolute url - full web site address

href=full url


#### links to other pages on same site, use relative URL

href= name of file if in same folder

#### email:

 href-"mailto:email.org" email

#### opening links in a new window

*target

a href -"http://www.imbd.com" target -"_blank"

#### linking to specific part of same page

identify in the headings where these links will be within the page

example

link will look like

&lt;a href-"#interlude"&gt;Interlude&lt;/a&gt;

header will look like

&lt;h2 id-"interlude"&gt;Interlude&lt;h2&gt;

### Chapter 5

#### importing image

&lt;img src-"where to find image"alt-"text

 description"title-"additional info about image" /&gt;

#### height and width of images

inside img

example width="600" height="450"

#### placement for images

before paragraph- new paragraph starts on new line after image

inside start of paragraph- first row of text indents to fit image

middle of a paragraph- image is between word it was place in writing

#### aligning

inside img align="left" or align="right"

align="top" align="middle" align="bottom"

###Three rules for images

1.save img in right format (jpeg,gif,png)

2.save at right size

3.use correct resolution

colors use jpeg

few colors or large area of same colors use gif or png

72ppi-resoltion


### Chapter 6

row by row

td or th is number of cells in row

use row span or colspan to span across more than one row

table open

tr (row) open
 column name = th scope-"col"name"
td (cell in row)open close

tr close

tr open

td open close

tr close

table close

### Chapter 7

allows you to collect information from visitors of site

search bars, shopping, mailing list, ect

#### Form controls

|Form Controls | Use |
|--------------|:-----:|
|Text Input|single line of text(emails or names)|
|Password Input|single line, masked characters(**)|
|Text Area|Multi-line text box for messages or comments|
|Radio Buttons|User must select one option(bubble)|
|Checkboxes|User can select or deselect one or more options|
|Drop-down Boxes|User must pick from list|
|Submit Button|Submit data from form to another webpage|
|Image button|colored submit button|
|File Upload| allows users to upload files to website|

Once filled and submitted forms go to a server along with values entered server sends back page

#### Form Structure

&lt;form action="URL for the page server will recieve"method="get"&gt;

  &lt;p&gt;USERNAME:

    &lt;input type="txt" name="username" size ="15" maxlength="30"/&gt;

  &lt;/p&gt;
  &lt;p&gt;Password:

  &lt;input type="password" name="password"size="15"maxlength="30"/&gt;

  &lt;/p&gt;

&lt;/form&gt;

methods:

get: short forms (search boxes just receiving data not adding to database)

post: allows user to upload file, very long, sensitive data(password), adds or deletes information

&lt;textarea name="comments" cols="20" rows="4"&gt;

#### input:

*type=text

name, size, maxlength

*type=password

name, size, maxlength

*type=Radio

name, value, checked

*type=Checkbox

name,value,checked

*type=file

name

*type=submit

name, value,

*type=image

src,width,height

----------------
*multiline

textarea name="" cols="" rows=""

*dropdown list

&lt;select name=""&gt;

 &lt;option value=""&gt;Displayed Name&lt;/option&gt;

&lt;/select&gt;


### buttons and hidden Controls

appearence of Buttons

combine text and images between opening and closing button Tags

hidden

&lt;input type=hidden name="bookmark" value="lyrics"
/&gt;

### labeling form Controls

group form elements

fieldset

[] &lt;-- basically puts text in table that looks like this

legend labels box^--

form validation

sends errors if form isnt correctly filled

*date

input type= "date" name="depart"

*email and url input

input type="email" name=email

input type=url"name="website"

*search

type=search name="search"

###Chapter 8

HTML 4-1997

XHTML 1.0-2000

HTML5-2000 &lt;!DOCTYPE html&gt;

*comments

&lt;!--comments go here--&gt;

*id Attributes

global Attributes used to identify specific paragraphs in html

*class Attributes

*block elements

h1

p

ul

li

*inline elements

continue on same line
a

b

em

img

*grouping text emlements in blocks

div group et of elements together

*iframes

mini window within page (map)

iframes

height

width

src

scrolling

frameborder

seamless

*information about your page

go in head elements

description

keywords

robots weather search engine should show page

author

pragma keeps browser from caching page

expires

*escape character page 201

### Chapter 9

*adding flash movie to webpage

location-replace-width-height-version


convert video to flv-find flv player to play-include

 the player and video in page

*adding video to pages

video src="path to video"
poster="image to show while video is downloading"
width=""
height=""
preload="none,auto, or metadata"
controls"own controls for playback"
loop"repeat video"

multiple video source page 222

src,type,codecs

*adding audio to web pages

use hosted service

use flash

use HTML5

add flash player

audio src=""controls autoplay

### Chapter 10

#### css

specifies how content should appear

selector and declaration  

p{
  font-family:Ariel;
  color:yellow;
}
placed after closing html

you can link in your css file using

&lt;link href="css/styles.css"type=text/css"rel="stylesheet"/&gt;

href=path,type=type of document,rel=relationship

Internal css define inside head

&lt;stlye type=text/css&gt;

&lt;head&gt;

body{

  font-family: arial;
  background-color:rgb;

}

hi{
  color:fkjhf;
}

*use external style sheet most times

selectors:

|selector|meaning|ex|
|--------|-------|--|
|universal|all elementsof document|*{}|
|type|matches element names|h1,h2,h3{}
|class|matches class|.note|
|id|matches id|#introduction|
|child|matches direct child|li&gt;a{}|
|descendant|??|p a {}|
|adjacent sibling|??|h1+p|
|general sibling|?|h1~{}|

###Chapter 11

####color

foreground color:

color: rgb values, hex codes, or color names.

background-color:

background-color:per section or for whole pages

check contrast

opacity:

value between 0.0 and 1.0

then add color

hsl, hsla

hsl(hue,sturation%,lightness%,alpha(transparecy) bw 0.0-1.0)

###chapter 12

####Text

font-family specifies font of Text

font-size is the size of the letters/words

pixels(px), percentages(%), or ems(em)

font face is where you can download a new font

src is the path to the font

format font

eot-IE

woff-chrome 6+

ttf/otf-firefox

svg

*bold

body{

font-weight:bold;

}

*italic

font-style:italic;

* text-transform

-uppercase

-lowerase

-capitalize (first letter of each word)

*underline and strike

text-decoration: none, underline, overline, line-through, blink

*leading

line-height:space between lines

*letter and word spacing

letter-spacing:space between letters

word-spacing:space between words

*alignment

text-align:left,right,center,justify

vertical-align:baseline,sub,super,top,text-top,middle,
bottom,text-bottom

*indenting text

text-indent:

*drop shadow

text-shadow:left and right, top and bottom,blur,color of drop shadow

*first letter or lines

:first-letter{

}

:first-line{

}

*styling links

:link color of link before clicked

:visited color of link after

*responding to users
:hover
:active
:focus

###chapter 13

box dimensions

width and height

div.box {
  height:
  width:
  background-color:
  ect:
}

max and min height and width(img)

min-width:
max-width:


min-height:
max:height:

overflow Content

overflow:hidden or scroll

*Border

border-width:thin,medum, thick

border-top,bottom,right,left-width

border-style:solid,dotted,dashed,double,groove,ridge,inset,outset

short hand border

border: width,style,color

*Margin

gap between boxes

*Padding

space between content and border

*display;inline,block,inline-block,none

*visibility:hidden, visibile

###chapter 14

table properties

list-style-type:

list-style-image:

list-style-position:

width,padding,transform,letterspacing,fotsize,border top and bottom, text-align,background-color,hover

Padding

hide or show borders on empty cell

spacing, collapsing

###chapter 15

####Position

*Normal FLow:down the pages

position:static;

*Relative Positioning: shifts an element

position:relative;

*absolute positioning

position:absolute;

*Fixed Positioning:
position:fixed;

*Floating elements:move to left or right as a block element

float:right;

side by side use float and width

clearing floats:

float:left;

.clear{

  clear: left;
}

*overlapping elements

position:Fixed

z-indez:10;

overflow:auto

### Chapter 16

-control image sizes:

img.large {

  width:500px

  height:500px
}

img.medium{

  width:250px
  height:250px
}
img.small{
  width:100px
  height:100px
}


-align images

img.align-left{

  float:left;

}
do for left right and center

-addding background images

body{

background-image:url("url");

}

### chapter 17

HTML 5 layout

header

footer

navigation (NAV)

article

aside

sections

heading groups(hgroup)

figures(figure, figcaption)

sectioning elements(div)

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
