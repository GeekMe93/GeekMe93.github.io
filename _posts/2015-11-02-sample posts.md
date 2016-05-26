---
layout: post
title: Sample post
categories: [tutorial]
tags: [sample, blog]
---

###  Message

<p class="message">
  Lorem ipsum dolor sit amet, ullum fastidii ei per. Aeterno elaboraret vix ne, vim ad legimus vocibus. Cu vis sonet graecis. Quis unum aeque ei est, duo no amet ullum choro.
</p>

### Lead paragraph
<p class="lead">
  Lorem ipsum dolor sit amet, ullum fastidii ei per. Aeterno elaboraret vix ne, vim ad legimus vocibus. Cu vis sonet graecis. Quis unum aeque ei est, duo no amet ullum choro.
</p>

### Summary

<div class="summary">
<div class="summaryHeader">Summary</div>
<div class="summaryBody">
Summary Content
</div></div>

### Typography

# Header 1

## Header 2

### Header 3 

#### Header 4

This is normal text.

**This is bold text**

***This is bold italic text***

`this is code`

[This is a link](#)


> This is quote

- item 1
- item 2
- item 3

* item 1
* item 2
* item 3

1. item 1
2. item 2
3. item 3

add a photo
![](http://i.imgur.com/4ojz1sG.gif)

### Table

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Upvotes</th>
      <th>Downvotes</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Totals</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>10</td>
      <td>11</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td>7</td>
      <td>9</td>
    </tr>
  </tbody>
</table>



## Inline HTML elements

HTML defines a long list of available inline tags, a complete list of which can be found on the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

- **To bold text**, use `<strong>`.
- *To italicize text*, use `<em>`.
- Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
- Citations, like <cite>&mdash; Mark otto</cite>, should use `<cite>`.
- <del>Deleted</del> text should use `<del>` and <ins>inserted</ins> text should use `<ins>`.
- Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.

Most of these elements are styled by browsers with few modifications on our part.

## Footnotes

This is an example of footnote [^fn-footnoteID] will lead you to a footnote. The syntax looks like:

{% highlight text %}
This is an example of footnote[^fn-footnoteID]
{% endhighlight %}

The syntax for the  list looks something like this:

{% highlight text %}
[^fn-footnoteID]: description about footnote.
{% endhighlight %}

You can place the footnoted content wherever you like. Markdown parsers should properly place it at the bottom of the post.


### Gists via GitHub Pages

Vestibulum id ligula porta felis euismod semper. Nullam quis risus eget urna mollis ornare vel eu leo. Donec sed odio dui.

{% gist 13f94b734a4ddb132735 gist.md %}



-----

[^fn-footnoteID]: description about the footnotes.


