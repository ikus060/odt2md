---
author: Patrik Dufresne
changed: '2015-10-27T17:21:42.709091490'
changedby: Patrik Dufresne
created: '2015-10-20T13:41:57.656627956'
description: 'This is some comments !'
generator: 'LibreOffice 4.3.3.2 (Linux)'
tags: [val1, val2']
layout: page
title: My Title
---

Typography
----------

Heading 1
---------

### Heading 2

#### Heading 3

##### Heading 4

###### Heading 5

### Example body text

Nullam quis risus eget [urna mollis ornare](http://localhost:4000/test1.html#) vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Nullam id dolor id nibh ultricies vehicula.

This line of text is meant to be treated as fine print.

The following snippet of text is **rendered as bold text**.

The following snippet of text is *rendered as italicized text*.

An abbreviation of the word attribute is attr.

Quotation
---------

> This is a block quote. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.

Code
----

~~~ western
from pandocfilters import toJSONFilter

def headers(key, value, format, meta):
  if key == 'Header' and value[0]==1:
      return []

if __name__ == "__main__":
  toJSONFilter(headers)
~~~

This is some inline code block: `key == 'header'`.

Tables
------

| \#  | Column heading                         | Column heading |
|-----|----------------------------------------|----------------|
| 1   | Column content<br/> With multiple Line | Column content |
| 2   | Column content                         | Column content |
| 3   | Column content                         | Column content |
|     |                                        |                |

List
----

### Unordered list of item

-   List item 1
-   List item 2
-   List item 3
-   List item<br/>with multiple line

### Ordered list of item

1.  One
2.  Two
3.  Three

Image
-----

![](test-1.jpeg)
