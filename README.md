Whiskey
=======

Whiskey is a simple test runner for NodeJS applications.

Features
========

* Each test file is run in a separate process
* Support for a test file timeout
* Support for a "failfast mode" (runner exits after a first failure)
* Nicely formatted output (colors!)

TODO
====

* Support for "TAP" output (http://testanything.org/wiki/index.php/Main_Page)

Screenshot
==========
![Console output](https://img.skitch.com/20110326-j5rk1damqt4yr7adw5mjqbqjd.jpg)

Dependencies
===========

* optparse-js
* async
* sprintf

Changes
=======

* 26.03.2011 - v0.2.0
  * Add support for the failfast mode (runner exists after a first failure)
  * User can specify custom test timeout by passing in the --timeout argument
  * Add support for a setUp and tearDown function
  * Add colors to the output
  * Now each test file must export all the test functions so the runner can
    iterate over them

* 25.03.2011 - v0.1.0
  * Initial release (refactor module out from Cast and move it into a separate
    project)

Installation
============

Install it using npm:
    npm install whiskey

Usage
=====

    whiskey --tests <test files> [options]

Example
=======

For examples check the `example` folder.
