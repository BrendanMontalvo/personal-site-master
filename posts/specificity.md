---
title: Intro to Specificity in CSS
description: This is a post on My Blog about Specificity.
date: 2022-04-19
tags:
  - CSS
layout: layouts/post.njk
---
CSS is the creative aspect of HTML that helps make what a user is looking at seem engaging and interesting. With that comes complications, and the ability to make changes and fix mistakes <em>should</em> be done in a clean manner.
My basic understanding of Specificity is that it is a concept that establishes a set of rules to help determine which methods of creating and editing styles get highest priority.
There are four ranks in which CSS code is given priority. Top priority is Inline CSS Styling. Inline CSS is when you apply the style code inside the HTML tag. 
I will give an example below, because this method of CSS styling is different from the rest in terms of where it is placed, in that it can only be placed in an html code-line.
`<p style="color: blue">`. 
The example above shows a paragraph html tag that has Inline style inside of it to determine the color of the paragraph it represents.
Inline CSS is generally frowned upon as it overrides everything else and is very rigid in its customization. Because of this, the rigidity may block the ability to target specific elements or classes within a code-block.
The second highest priority is using code ID's and the 3rd being classes and last being elements.
All three of these methods can both be used in <strong>Internal CSS</strong> and <strong>External CSS</strong>.
Ideally, a developer should try to create classes and target elements when styling in CSS, using Internal CSS or External CSS, to keep code clean, and be able to target specific code in your HTML. Another thing to remember is that each level of priority is only relevant to that level. For example, you can have an infinite number of ID's used as a reference to create styles in your HTML, but if you use Inline CSS styling, it will override all the ID's you had referenced in your code. The  If you use 5 ID's to make a change it will override a style that used 4 ID's. With that said it is important to understand the heirarchy more so than it is to understand the "number" value.