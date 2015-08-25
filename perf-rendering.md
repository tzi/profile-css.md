# CSS rendering performance

CSS rendering performance is the efficiency to compute styles after everything is loaded.
The purpose is to get fluid interfaces, for example fast scrolls or **smooth animations**.
Todo that we need to get the browser rendering the page at **60fps everywhere**.


## What actually happens in the browser? 

There’s no universal solution to improve render performance, it depends on your use-case.
The best beginning is to understand the steps which the browser has to do to get pixels onto the screen.

 * [Optimising for 60fps everywhere (Article)][gosquared-article]

> GoSquared wrote presentations and code examples to explain the concepts of **re-layouts, re-paints, layers, composition, CPU and GPU**.

[gosquared-article]: https://engineering.gosquared.com/optimising-60fps-everywhere-in-javascript


 * [CSS animations and transitions performance: looking inside the browser][adobe-animations-performance]
  
> Adobe explains why it is cheaper for the browsers to animate a transformation than an element height.

[adobe-animations-performance]: http://blogs.adobe.com/webplatform/2014/03/18/css-animations-and-transitions-performance/


## Experience Feedback

 * [GitHub's CSS Performance (Slides)][github-slides] or [(Video)][github-video]

> GitHub had some pages with *almost 30s of style recalculation (slide 19)*,
because of particular conditions like *50k DOM elements (slide 63)*.
In this hard context, they had to drastically simplify their HTML and CSS.

> One of the best point is that *less than half of the people that touch the CSS (slide 101)* are *CSS developers (slide 102)*.
So you have to have rules and tools to monitor your CSS, like the number of selectors. 

[github-slides]: https://speakerdeck.com/jonrohan/githubs-css-performance
[github-video]: https://vimeo.com/54990931




