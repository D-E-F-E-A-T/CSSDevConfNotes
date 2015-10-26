# CSS Dev Conf
----------------
# Sara Soueidan -- Opening Keynote
## SVG For Web Designers and Developers

Last name: Swaidaan
SVG is the preferred format for images like user interface elements like vector based stuff
Don't choose Svg when it's going to affect performance in a bad way
SVG

  - Icon Systems
  - Ad banners
  - Infographics
  - Data visualizations
  - Animated Illustrations
  - Filter effects (on SVG as well as HTML elements, including text)
  - Simple UI shapes and arbitrarily-shaped UI components

PostCSS Custom @-rule https://github.com/jonathantneal/postcss-write-svg

Communication = <3

 - Use SVGO for optimizing SVGs
  + https://github.com/svg/svgo
  + can break svgs
  + *replaces* file 
  + svgomg online tool
    - https://jakearchibald.github.io/svgomg/
- Inkscape offers more options that yield cleaner code


Spriting Techniques 

  - \<use\> 
    + Multiple SVGs are combined into one file using \<symbols\>
    + \<use link:href="icons.svg#icon-name"\>\</use\> within svg
    + can't select specific elements to style. stuff brought in by \<use\>s is put inside the shadow dom and can't be selected.
    + variants can be accomplished with CSS Variables... which are only supported in FF
  - svgView method
    + \<img src="icons.svg#svgView(viewBox(x,y,z,etc))"\>
  - \<view\> method
    + \<img src="icons.svg#view-name"\>
  - background method
    + grumpIcon

goto svg animation library: http://greensock.com/svg-tips

\<object\>

codepen chrisgannon/blog/my-first-svg-banner-ad