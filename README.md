Uniwheel
========

A unified cross browser mouse wheel event handler. Supports listener removal.

Further study: https://developer.mozilla.org/en-US/docs/Web/Reference/Events/wheel


Usage:
------

		var wheel = require('uniwheel');

		function onWheel(e) {
		  e.preventDefault();
		  console.log(e);
		}

		//arguments: element, cb, useCapture
		wheel.on(window,onWheel,false);
		wheel.on(window,onWheel,true);

		setTimeout(function(){
		  wheel.off(window,onWheel,false);
		},2000);

		setTimeout(function(){
		  wheel.off(window,onWheel,true);
		},4000);


License:
--------
MIT