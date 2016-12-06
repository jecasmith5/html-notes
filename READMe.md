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

table open

tr (row) open
 column name = th scope-"col"name"
td (cell in row)open close

tr close

tr open

td open close

tr close

table close
