ng-shortcut
===========

An Angular.JS directive to bind keyboard shortcuts to DOM elements.


Installation
------------

Using Bower:

    $ bower install ng-shortcut --save

Include the JavaScript code somewhere in your HTML code:

    <script src="/path/to/ng-shortcut.js"></script>

Add **ngShortcut** as a module dependency to your app:

    angular.module('myApp', [
        'ngShortcut',
        'myApp.MyCtrl'
    ])


Usage
-----

You can bind keyboard shortcuts to HTML elements like this:

    <button shortcut="...">Button</button>

Possible values for the `shortcut` attribute are:

* a key code, like `32` for the space key
* a list of key codes separated by comma, like `32,13` for space or enter key
* a key code with a modifier key, like `alt-65` for Option+A
* a number of key codes with modifiers, left as an exercise for the reader

A tiny tool to help you find out which key codes to use can be found [here](http://keycoder.pbsit.es/).


### Triggered event

By default the `click` event will be triggered when the specified shortcut is used. You can configure a different event to be triggered by using the additional `shortcut-event="focus"` attribute.


License
-------

[MIT](http://philippbosch.mit-license.org/)
