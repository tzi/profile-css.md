CSS rendering performances
======

Experience Feedback
------

GitHub's CSS Performance [Slides][github-slides] - [Video][github-video]

> GitHub had some pages with [almost 30s of style recalculation][github-slow],
because of particular conditions like [50k DOM elements](github-context).
In this hard context, they had to drastically simplify their HTML and CSS.

> One of the best point is that [less than half of the people that touch the CSS][github-team] are [CSS developers][github-team-css].
So you have to have rules and tools to monitor your CSS, like the number of selectors. 

[github-slides]: https://speakerdeck.com/jonrohan/githubs-css-performance
[github-video]: https://vimeo.com/54990931
[github-slow]: https://speakerdeck.com/jonrohan/githubs-css-performance?slide=19 
[github-context]: https://speakerdeck.com/jonrohan/githubs-css-performance?slide=63
[github-team]: https://speakerdeck.com/jonrohan/githubs-css-performance?slide=101
[github-team-css]: https://speakerdeck.com/jonrohan/githubs-css-performance?slide=102




