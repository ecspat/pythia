Pythia: Smart Completion for JavaScript
=======================================

This is an implementation of smart completion for JavaScript using combined static-dynamic analysis.

This project just contains high-level driver code, the actual cleverness happens in the DAIN and ecsptr projects on which it depends.

Installation
------------

Run `npm install` in this directory to pull in dependencies.


Usage
-----

        node complete.js file.js

Look for an expression `e.$$f` in `file.js` and see whether we would be able to suggest `f` as a completion for receiver expression `e`. Prints out the result and some statistics.

If you pass an HTML file instead of a JavaScript file, all JavaScipt files included by `script` tags will be considered.

Note that you have to manually replace frameworks with their instrumented versions at the moment.
