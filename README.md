# Web Performance Project


## How to run the application
1. Download the GitHub zip file or clone the repository onto your local workstation:
	* Location:  [https://github.com/monicamucajal/frontend-nanodegree-mobile-portfolio/](https://github.com/monicamucajal/frontend-nanodegree-mobile-portfolio/ "My mobile portafolio")
2. Open a browser window and navigate to the "index.html" and "pizza.html" files in your application's directory.


## index.html Optimizations
1.	Loading the external Google font via inline CSS.  Only used “/*latin/” since the Google page mentioned that “Latin” is the one supported by all fonts.
2.	Moved “style.css” inline so the reference to “style.css” could be removed.
3.	Moved print.css reference to the end  <link href="css/print.css" rel="stylesheet">  to delay loading of it until after the page loads.
4.	Added “async” to Google Analytics reference in script tag so end user does not wait for Google Analytics.
5.	Used Photoshop to optimized for web the very large “pizzeria.jpg” image.

New PageSpeed Score:  92/100


## main.js Optimizations

1.	Changed to use “getElementById” and “getElementsByClassName instead of querySelector/querySelectorAll in multiple places
2.	Created a new array to store elements with class randomPizzaContainer
3.	Moved declaration of variables outside the for loops (“dx”, “newWidth”, “pizzasDiv”, “scrollTop”, “movingPizzas”, etc. )
4.	Changed for loop for addEventListener to only executed till 48 instead of 200.


## pizza.html Optimizations
1.	Inlined the styles.css style
2.	Updated “The Udacity Special” and “The Cameron Special” to use bootstrap “col-md-6” instead of percentages.


## Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api"). We didn't cover the Navigation Timing API in the first two lessons but it's an incredibly useful tool for automated page profiling. I highly recommend reading.
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>


## Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>
