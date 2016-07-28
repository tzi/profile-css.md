# CSS rendering performance in 10 links

CSS rendering performance is the efficiency to compute styles after everything is loaded.
The purpose is to get fluid interfaces, for example fast scrolls or **smooth animations**.
To do that we need to get the browser rendering the page at **60fps everywhere**.


## Is it important?

 * Adam Morse, [Does CSS Performance Matter?][mrmrs-caring] Article published December 18, 2014.
 
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


## CSS selectors performance

 * Steve Souders, [Performance Impact of CSS Selectors][stevesouders-selector]. Article published March 10, 2009.

> The possible performance gains from optimizing CSS selectors will be small, and are not worth the costs.

[stevesouders-selector]: http://www.stevesouders.com/blog/2009/03/10/performance-impact-of-css-selectors/


## Tools

 * [CSS Triggers][csstriggers]. Website.
 * Paul Lewis, [CSS Triggers] [csstrigers-post]. Article updated July 26, 2014.
 
> He wanted to create a tool that would allow developers to more readily understand the ramifications of changing their styles.
And now it is the most important tool to have when dealing with CSS rendering performance issues.

[csstriggers]: http://csstriggers.com/
[csstrigers-post]: https://aerotwist.com/blog/css-triggers/


## Experience Feedback

 * Jon Rohan (GitHub), [GitHub's CSS Performance][github-slides]. Slide published December 5, 2012 on Speaker Deck.
 * Jon Rohan (GitHub), [GitHub's CSS Performance][github-video]. Video published December 5, 2012 on vimeo.

> GitHub had some pages with *almost 30s of style recalculation ([slide 19](https://speakerdeck.com/jonrohan/githubs-css-performance?slide=19))*,
because of particular conditions like *50k DOM elements ([slide 63](https://speakerdeck.com/jonrohan/githubs-css-performance?slide=63))*.
In this hard context, they had to drastically simplify their HTML and CSS.

> The most interesting point is that *less than half of the people that touch the CSS ([slide 101](https://speakerdeck.com/jonrohan/githubs-css-performance?slide=101))* are *CSS developers (s[lide 102](https://speakerdeck.com/jonrohan/githubs-css-performance?slide=102))*.
So you have to have rules and tools to monitor your CSS, like the number of selectors. 

[github-slides]: https://speakerdeck.com/jonrohan/githubs-css-performance
[github-video]: https://vimeo.com/54990931


 * Chris Ruppel (Four Kitchens), [Fix scrolling performance with CSS will-change property][fourkitchens-scrolling]. Article published July 1, 2015.

> Four Kitchens’ website had a big fixed background image that cause scrolling performance issues.
This article show how they diagnose it and fixed it.

> It is a typical use case that is certainly present in one of your projects.

[fourkitchens-scrolling]: https://fourword.fourkitchens.com/article/fix-scrolling-performance-css-will-change-property


 * Ross Allen (AirBnB), [CSS box-shadow Can Slow Down Scrolling][airbnb-box-shadow]. Article published November 11, 2011.

> An example from the AirBnB dashboard, with real metrics, show that blur-radius cost processing power.

[airbnb-box-shadow]: http://nerds.airbnb.com/box-shadows-are-expensive-to-paint/


## Not referenced links

 * http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/
 * http://www.html5rocks.com/en/tutorials/speed/unnecessary-paints/
 * http://paulbakaus.com/tutorials/performance/the-illusion-of-motion/
 * http://benfrain.com/browser-representatives-on-css-performance/
 * http://meiert.com/en/blog/20090312/performance-of-css-selectors/
 * http://www.smashingmagazine.com/2012/06/play-with-hardware-accelerated-css/
 * http://calendar.perfplanet.com/2014/hardware-accelerated-css-the-nice-vs-the-naughty/
 * https://github.com/axemclion/browser-perf
 * http://gent.ilcore.com/2011/03/how-not-to-trigger-layout-in-webkit.html
 * https://github.com/wilsonpage/fastdom
 * http://www.kellegous.com/j/2013/01/26/layout-performance/
 * http://www.thecssninja.com/javascript/pointer-events-60fps
 * http://www.thecssninja.com/javascript/follow-up-60fps-scroll
