# CSS rendering performance

CSS rendering performance is the efficiency to compute styles after everything is loaded.
The purpose is to get fluid interfaces, for example fast scrolls or **smooth animations**.
Todo that we need to get the browser rendering the page at **60fps everywhere**.


## Is it important?

 * Adam Morse, [Does CSS Performance Matter?][mrmrs-caring] Article published December 18, 2015.
 
> Yes it does. 
 
[mrmrs-caring]: http://xn--h4hg.ws/2014/12/18/caring/


## What actually happens in the browser? 

There’s no universal solution to improve render performance, it depends on your use-case.
The best beginning is to understand the steps which the browser has to do to get pixels onto the screen.

 * JT (GoSquared), [Optimising for 60fps everywhere][gosquared-article]. Article published July 10, 2014.

> Presentations and code examples to explain the concepts of re-layouts, re-paints, layers, composition, CPU and GPU.

[gosquared-article]: https://engineering.gosquared.com/optimising-60fps-everywhere-in-javascript


 * Max Vujovic (Adobe), [CSS animations and transitions performance: looking inside the browser][adobe-animations-performance].
 Article published March 18, 2014.
  
> Why it is cheaper for the browsers to animate a transformation than an element height.

[adobe-animations-performance]: http://blogs.adobe.com/webplatform/2014/03/18/css-animations-and-transitions-performance/


## Experience Feedback

 * Jon Rohan (GitHub), [GitHub's CSS Performance][github-slides]. Slide published December 5, 2012 on Speaker Deck.
 * Jon Rohan (GitHub), [GitHub's CSS Performance][github-video]. Video published December 5, 2012 on vimeo.

> GitHub had some pages with *almost 30s of style recalculation (slide 19)*,
because of particular conditions like *50k DOM elements (slide 63)*.
In this hard context, they had to drastically simplify their HTML and CSS.

> One of the best point is that *less than half of the people that touch the CSS (slide 101)* are *CSS developers (slide 102)*.
So you have to have rules and tools to monitor your CSS, like the number of selectors. 

[github-slides]: https://speakerdeck.com/jonrohan/githubs-css-performance
[github-video]: https://vimeo.com/54990931


 * Chris Ruppel (Four Kitchens), [Fix scrolling performance with CSS will-change property][fourkitchens-scrolling]. Article published July 1, 2015.

> Four Kitchens’ website had a big fixed background image that cause scrolling performance issues.
This article show how they diagnose it and fixed it.

> It is a typical use case that is certainly present in one of your projects.

[fourkitchens-scrolling]: https://fourword.fourkitchens.com/article/fix-scrolling-performance-css-will-change-property




