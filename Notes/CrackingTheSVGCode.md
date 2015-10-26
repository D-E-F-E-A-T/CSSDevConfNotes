# CSS Dev Conf
----------------
# Brenda Storer
## Cracking the SVG Code #CrackSVG

504-229-6828

###why svg?

  - Vector graphic, infinitely scalable
  - Small byte size, can even gzip
  - we can use them like a bitmap
  - or use them inline!

###what is familiar from html?

  - it's xml
  - it's like an html document for digital drawings
    + unicode characters
    + element tags and attrs
    + white spcae unimportant
    + nesting
    + bitmaps, anchors, text
    + shapes, paths, opacity, gradients, rotation, anmiation


###development history

  - 90s: macromedia and microsoft introduced vml
  - adobe and sun submitted a competing format known as pgml
  - w3c developed svg. 1998

###name spacing

  - provides semantic meaning for the name of that element and its children, provided that the children do not have their own name spaces
  - its value can be any string but usually url
  - the links often can go nowhere
  - attributes can have namespaces too
  - it's a good thing to keep around

###title and desc in svg

  - think of \<title\> like the `alt` attr

###viewports

  - unites can be rem, em, ex, px, pt, pc, cm, mm in
  - shapes inside of svgs use same units
  - it's all relative

###stuff you can delete from generated svgs

  - \<?xml\> declaration
  - version
  - xml:preserve -- for text
  - namespaced stuff is likely referenced
  - enable-background 


###svg paths

  - m = movemto (x,y)
  - l = lineto (x,y)
  - a = arc )rx, ry, x-axis-rotation, large-arc-flag, sweep-flag)
    + exual rx and ry mean a circular arch, different mean ellipses
  - c = curveto (cubic bezier curve)
  - s = curveto (smooth or shorthand cubic bezier curve)
  - uppercase and lowercase are different

###cubic bezier curve

  - c x1,y1 x2,y2 x,y
  - s x2,y2 x,y


  - transform svg attr is more supported than css transform style