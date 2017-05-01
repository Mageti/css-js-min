# css-js-min
Small python scripts to minify CSS and JS

## License
"Beerware" license

## Inspiration
Freely copied and inspired by https://github.com/zacharyvoase/cssmin and https://github.com/isaacs/cssmin

# Usage
## How to use
Use it from the command-line:

    $ cssmin --help
    $ cat file1.css file2.css file3.css | cssmin > output.min.css
    $ cssmin --wrap 1000 < input.css > output.css

Or use it from Python:

    >>> import cssmin
    >>> output = cssmin.cssmin(open('input.css').read())
    >>> print output

## When to use
When you want, but concider that it is discouraged to use it on the fly, because of its performances.
I personnaly use it when I deploy a new version of my websites: each new deployment triggers a call to these scripts.