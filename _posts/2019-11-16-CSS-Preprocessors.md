---
layout: post
date: 2019-11-16 10:23:10 -0600
categories: 1dv022
comments: true
---

### Thoughts on using preprocessing CSS

With the ability to preprocess the CSS you get a lot more freedom to shorten and simplify the code. To be able to use variables is alone a big deal for developers since it makes creating and maintaining so much easier. You can change the color theme of the whole project just by editing the variables, or use variables as arguments in mixins (Sass version of functions) to make it possible to include whole sections of code just by calling that mixin in however many places you like.

Comparing to vanilla CSS, a preprocessor can be a bit cumbersome to set up, but the hassle is worth it. You dont have to repeat yourself nearly as much since with regular CSS you cant use nesting and you cant use calculations nor variables. The best of both worlds would be if CSS implemented all the pros of preprocessed CSS and got rid of all the cons with vanilla CSS.

![Image of preprocessor logos]({{ site.url }}/assets/css_prepro.png)

In this project I used the minima Jekyll theme and edited it to my liking. The theme uses mixins, variables, nesting and the theme is built with several .scss files that are "included" in the main stylesheet. That makes it easier to keep track of the code since you are able to categorize sections of the code to separate files.

Pros with preprocessing CSS are already mentioned above, but what about the cons? The first downside I have come across is that it becomes harder to debug. Thats because the very nature of preprocessed CSS where you write for instance Sass and that in turn becomes "compiled" or translated into CSS. That makes finding the row number where the faulty code is very hard since it does not correspond to the code written your in Sass file. Another con is that it adds a step to the workflow where you explicitly have to compile or translate to CSS. Preprocessing can also generate very large CSS files, that takes away some of the control if you aim to reduce the size of your project. Another con could be that using a preprocessor requires an additional tool and knowledge about the syntax. The best option would be for CSS to adopt the way of thinking that a preprocessor use. Hopefully that is not too far off into the future.
