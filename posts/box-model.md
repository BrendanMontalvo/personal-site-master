---
title: Basics of Box Model
description: This is a post on My Blog about Box Model.
date: 2022-04-20
tags:
  - CSS
layout: layouts/post.njk
---
<p class="intro">The Box Model is how elements are displayed on an html page. All elements in a page is going to occupy it's own "box". There are different ways of adding space to an element. Below is an attempted example:</p>
<p class="example">
<style>
    .example {
        border: 25px solid red;
        border-bottom-color: yellow;
        padding: 25px;
        margin: 50px;
        text-align: center;
    }
</style>
Box of content
</p>
<p> In the box of content created above, the padding is the space that is inside the box, and the margins are the space outside the box, in this instance it is the space between the box of content and this text. The red and yellow borders can be created similarly by using `border: 25px solid red` which would create an all red solid border about 25px wide, I created a border to help to visualize the space between content.

<p>You can also modify the width and length of a box, but be careful, if you modify the width of a box the content can "spill-out" and thus create something that won't automatically keep inside the box. Same goes for length.

<h2>Shorthand Method</h2>
<p>Shorthand method is important to understand as it is a shorter way of creating code for your margins, padding and borders. All 3 methods of styling can use the same concept.
<p>Here is an example of shorthand using margins below:<p>
<p><code>margin-top: 10px;</p>
<p>margin-left: 10px;</p>
<p>margin-right: 10px;</p>
<p>margin-bottom: 10px;</code></p>
<p>This would be the long form way of creating a 10px margin for all four sides of the content box.

<p>The shorthand version:</p>
<p><code>margin: 10px</code></p>

<p>By inputing 10px only once, the code is automatically going to assume that it means for top, left, right and bottom. However, what if you wanted top and bottom to be the same and right and left to be the same but they have different values?</p>
<p>Well, this is what it would look like below:</p>
<p><code>margin: 10px 25px;</code></p>
<p>How the example reads out is that the 10px represents the top and bottom margin, and 25px represents the left and right margin.</p>

<p>You can play with this a couple of other ways as well, the simplest being if you had four different values for top, right, bottom, and left</p>

<p><code>margin: 10px 20px 30px 40px</code></p>

<p>Or, if you wanted top and bottom to be different values but right and left are the same?</p>
<p><code>margin: 10px 25px 5px</code></p>
<p>This code would read out with the 10px representing the top, 25px representing left and right, and 5px representing the bottom</p>

<p>It is important to understand this concept of shorthand as many methods of styling can use shorthand, and once you understand how to do it for one, you can do it for all different styles that utilize this such as padding and borders.</p>

<footer>Last little note: There is also something called <strong>auto</strong> which you can set right and left margins to so that space is filled, but you cannot use auto for top and bottom.