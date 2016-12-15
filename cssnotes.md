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
