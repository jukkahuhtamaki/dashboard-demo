README.md

## The first visualization widget: Highcharts ##

Let's start with a review of existing dashboards. Social media analytics is a prime example of a business domain in which web-based dashboards are the standard approach:

* Meltwater: http://www.meltwater.com/fi/products/
* Pulsar: http://pulsarplatform.com/

### Benchmark: creating a visualization with Tableau Public

* WYSIWYG tools exist for creating visualizations
* Examples include Tableau and Microsoft PowerBI
* What do consider to be key issues in developing visualizations with these kinds of tools?

### Implementing the first visualization ###

* Basic line chart: [Highcharts](http://www.highcharts.com/demo/line-basic)
* Use jsFiddle to change the data and appearance: http://jsfiddle.net/gh/get/jquery/1.9.1/highslide-software/highcharts.com/tree/master/samples/highcharts/demo/line-basic/
* E.g. montly average temperature in Tampere: http://ilmatieteenlaitos.fi/tilastoja-vuodesta-1961

Protip before we begin: you can start up our own local HTTP server with Python:

	python -m SimpleHTTPServer 8080 &

### Make the visualization dynamic

* Create a separate JSON file for visualization data
* Utilize jQuery to read the data from a file when the visualization is opened

### Integrate the visualization to a Node.js application

* How to serve JSON in a dynamic way by the Node.js application?
* How to integrate Highcharts to application that uses Jade template engine?
* How to use Hightcharts in Vue.js-based applications?

### Dashboard project ingredients ###

Starting your own project:

1. Create an HTML document.
1. Install Highcharts: http://www.highcharts.com/docs/getting-started/installation
1. Add an element for the visualization view.
1. Add the actual code that implements the visualization.

Making the dashboard look like a dashboard:

1. Download Bootstrap: http://getbootstrap.com/getting-started/#download
1. Use the dashboard template: https://getbootstrap.com/examples/dashboard/

### Dashboard features ###

Dashboards are a way to implement interactive visual analytics with web technologies. (Not all dashboards are implemented with web technologies though.)

Heer and Shneiderman (2012) give an insightful overview of features and functionalities related to interactive visual analytics: http://dl.acm.org/citation.cfm?id=2133821

Linking and brushing is one of the key features enabling exploration. Referrring to Becker and Cleveland (1987), Heer and Shneiderman (2012) note: "Brushing and linking is the process of selecting (brushing) items in one display to highlight (or hide) corresponding data in the other views." 

### Interconnected views in JS ###

DC.js introduces a particularly expressive way to implement dashboards in JS:  

Online manual is available for implementing your first dashboard: https://dc-js.github.io/dc.js/

The implementation is non-trivial, yet manageable with some knowledge on JS and the basics of web development.