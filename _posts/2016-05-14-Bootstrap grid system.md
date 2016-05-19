---
layout: post
title: Bootstrap grid system
categories: [Bootstrap]
tags: [notes, html, css, JavaScript]
---

I only listed important points in the grid system:

- the range of screen size;
- break points;
- container, row, and col;


### Classification of the screen size

- extra small screen (<768 px)
- small screen (768 px < w < 992 px)
- medium screen (992 px < w < 1200 px)
- large screen (> 1200 px)

### Break points

Important break points usually happens the critical points of screen size.
Break points work from smallest break points first to large

### Col

12 col grid system is used in Bootstrap. we have the following predefined class.

`col-(xs, sm, md , lg)-#`

> - xs - extra small
> - sm - small 
> - md - medium
> - lg - large
> - `#` any number from 1 to 12

### Example

1. we set the medium screen col in this example, when the screen size is shrink to small or extra small, all the horizontal col will stack with each other; 

2. We set both lg and xs col, let's think from small to large:

- extra small: take the xs col setting;
- small: still take the xs col setting;
- medium: still take the xs col setting;
- large: lg col will be applied under large screen;

We can see that the grid system is the basis for responsive design in Bootstrap.


