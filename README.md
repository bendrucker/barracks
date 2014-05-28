# Barracks

[![Build Status](https://travis-ci.org/yoshuawuyts/barracks.svg)](https://travis-ci.org/yoshuawuyts/barracks)
[![Coverage Status](https://coveralls.io/repos/yoshuawuyts/barracks/badge.png?branch=master)](https://coveralls.io/r/yoshuawuyts/barracks?branch=master)

An event dispatcher for the [flux architecture](http://facebook.github.io/react/blog/2014/05/06/flux.html).

## API
````js
// Initialize a dispatcher
var Dispatcher = require('barracks');
var dispatcher = Dispatcher();

// Register a new object:
var callbackFunction = function(arg) {
  /*side effect goes here*/
};
dispatcher.register('eventName', callbackFunction);

// Dispatch registered callbacks for 'eventName'
dispatcher.dispatch('eventName');
````

## License
[MIT](https://tldrlegal.com/license/mit-license) © [Yoshua Wuyts](yoshuawuyts.com)