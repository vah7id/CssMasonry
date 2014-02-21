CssMasonry
==========

Pure CSS Masonry Responsive Layout

If you have seen pinterest, they has a multi-column interface to display the pins and those pins arrange nicely even if they are not of the same height. They do it by using javascript to calculate the height of each pin and then positioning them absolutely. Achieving the same with CSS can be done in two ways:

<b>Using Floats</b>: Floats can be used but only if all the pins have same height otherwise there will be gaps left all over.
<b>Using CSS3 Columns</b>: This is what I used here. It is explained in detail below.

We Using CSS3 Columns solution in CssMasonry plugin :)


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
      


