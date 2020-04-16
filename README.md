# Simple logger: for easily switching all prints of a function on and off.

I wanted a printing function which could easily be turned off or on.
This is especially useful when debugging, or when one wants to create a function where the user has the option to see the inner workings of the function by using an input variable such as `printing`.

The famous logging module provides a Logger class, but it is an overkill. Using that module, I defined a few functions which do what I wanted:

1. `log` is the main function, acting as the printing function.
2.  `logger_switch` turns the logger on or off, depending on the arg. It also records the previous state of the logger.
3. `logger_cleanup` reverts the logger to its previews state, using the information recorded by `logger_switch.

With these one can construct functions with optional logging/printing.

#### Example:
<div style="text-align:center"><img src="example_logger.png" /></div>


