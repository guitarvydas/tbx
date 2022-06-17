usage: make

converts transpiler.tbx to transpiler.js in 3 steps:
1. uses comp.ohm + comp.fmt to create /tmp/js-comp1 which is the transpiled JS file, still containing verbatim and bracketed names
2. use name.ohm + js-name.fmt to convert bracketed names to JS format in /tmp/js-comp2
3. use verbatim.ohm + verbatim.fmt to strip verbatim brackets into transpiler.js
