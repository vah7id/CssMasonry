CssMasonry
==========

Pure CSS Masonry Responsive Layout

If you have seen pinterest, they has a multi-column interface to display the pins and those pins arrange nicely even if they are not of the same height. They do it by using javascript to calculate the height of each pin and then positioning them absolutely. Achieving the same with CSS can be done in two ways:

<b>Using Floats</b>: Floats can be used but only if all the pins have same height otherwise there will be gaps left all over.

<b>Using CSS3 Columns</b>: This is what I used here. It is explained in detail below.

We Using CSS3 Columns solution in CssMasonry plugin :)

Requirements
==============

Nothing :)

Usage
==========

It's so simple !
First step: adding cssmasonry.css file to our project :


      <link rel="stylesheet" href="../CssMasonry.css" />
      

Second step: adding html template of cssMasonry to your html file :


    <div class="wrapper">
      <div class="columns">
        <div class="item">
          ....
        </div>
        <div class="item">
         ...
        </div>
      </div>
    </div>
      

Now on to the styling:


.columns {
    -moz-column-count: 3;
    -moz-column-gap: 10px;
    -moz-column-fill: auto;
    -webkit-column-count: 3;
    -webkit-column-gap: 10px;
    -webkit-column-fill: auto;
    column-count: 3;
    column-gap: 15px;
    column-fill: auto;
}

column-count is a count of items in each column of our layout. and it can change in each media queries.
coulmn-gap is distance of every columns together.
      
and .item class is your boxes in each columns. you can place your css styles in this class about each boxes. 

For good measure, I added some media queries to adjust the number of columns depending on browser width:


@media (min-width: 320px) and (max-width: 500px) {
	.columns {
		-webkit-column-count: 2;
		-moz-column-count: 2;
		column-count: 2;
	}
}

@media (min-width: 500px) and (max-width: 768px) {
	.columns {
		-webkit-column-count: 3;
		-moz-column-count: 3;
		column-count: 3;
	}
}


This won't work in Internet Explorer 9 and below as it don't support multi column. However, you can use it if you don't care about it ;)
Make sure to take a look at the source code to understand more about it's working.

Demo
==============

http://vah7id.com/project/CssMasonry/DEMO/

License
==============

Copyright (C) 2012 Vahid Taghizadeh (vah7id@gmail.com)
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
