
Using:

* Webpack for build
* npm for JS dependencies
* venv for Python environment
* [Turbolinks](https://github.com/turbolinks/turbolinks/) to make the browser fast
* StimulusJS for JS application
  * babel because it was required by StimulusJS
* Flask for webserver

Testing:

1. You can see when you click links between the two pages, in the network tab
   it is an XHR request, not a full page load. This is turbolinks in action.
   Turbolinks intercepts clicks and switches out the <body> and checks
   [for other things](https://github.com/turbolinks/turbolinks#navigating-with-turbolinks).
1. Click the button, you'll see that StimulusJS controller updates the <span>

Flask:

* [Flask Quickstart](https://flask.palletsprojects.com/en/1.1.x/quickstart/)

StimulusJS:

* [Handbook](https://stimulusjs.org/handbook/hello-stimulus)
* [Starter Kit](https://github.com/stimulusjs/stimulus-starter/)

To run the server:

```
npm install
npx webpack;export FLASK_ENV=development FLASK_APP=app.py;flask run
```
