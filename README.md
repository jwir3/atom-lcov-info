## Atom lcov-info

### What

Displays code coverage information inside Atom based from information contained in an LCOV formatted file.

Using the current open file as a starting point, it traverses up the tree until the `coverage/lcov.info` file is found. As an example, while editing `/Users/joe/Projects/xyz/src/client/test.coffee` coverage information could be pulled from either `/Users/joe/Projects/xyz/src/coverage/lcov.info` or `/Users/joe/Projects/xyz/coverage/lcov.info`. (First match as found.)

![Coverage with line highlight](https://raw.githubusercontent.com/jacogr/atom-lcov-info/master/screenshots/coverage-01.png)

It supports LCOV information as generated by tools such as Mocha, Karma, Istanbul, and others.

### Why

Some reasons why this package might fit the bill for you -

- Coverage information can be toggled for all views using `ctrl-alt-c`
- There is no additional configuration, your `coverage/lcov.info` file is automatically located
- Highlights are configurable to either show as a line (default) or in the gutter (less obtrusive)
- Both relative and absolute file paths outputs in the `lcov.info` file are supported
- It does matching irrespective of the platform, i.e. mix-and-match of / and \ style paths are supported
- A summary of the total coverage per line is displayed on the statusbar
- A overall project summary is available, along with at-point views of the different project files
- Covered lines are highlighted in green, uncovered lines in red
- Coverage display can be configured for gutter-only, line & gutter
- Unobtrusive options to only display uncovered lines are available
- Has been tested with Karma, Mocha and Istanbul outputs

### How

Run your tests, generate a `coverage/lcov.info` file, toggle the coverage plugin and it displays.

### Where

The Atom package can be found on the Atom registry, [https://atom.io/packages/lcov-info](https://atom.io/packages/lcov-info).

Pull requests, issues, feature requests are all welcome and encouraged via [https://github.com/jacogr/atom-lcov-info](https://github.com/jacogr/atom-lcov-info).

### More

![Coverage with gutter highlight](https://raw.githubusercontent.com/jacogr/atom-lcov-info/master/screenshots/coverage-02.png)
