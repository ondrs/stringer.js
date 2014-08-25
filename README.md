# Stringer.js [![Build Status](https://travis-ci.org/ondrs/stringer.js.svg?branch=master)](https://travis-ci.org/ondrs/stringer.js)

Swiss knife for easy and immutable manipulation with strings in javascript.

## How to install
```
npm install stringer.js
bower install stringer.js
```

## How to use

Construct a new Stringer object

    var str = s('Hello! I am Stringer and I cost exactly $0! ♥');

And use as follows

    str.justNumber().toInt();
    // 0

    str.only(18).justLetters().toUpper().only(14).toString();
    // HELLOIAMSTRING

    str.webalize().toString();
    // hello-i-am-stringer-and-i-cost-exactly-0

    str.toTruncated(5);
    // Hello…

## Available methods

- justLetterAndNumbers
- justLetters
- justNumbers
- justDecimals
- removeDiacritics
- webalize
- rtrim
- ltrim
- lpad
- rpad
- escapeRegExp
- toUpper
- toLower
- only
- thousands
- isNumber
- contains
- toFloat
- toInt
- toString
- toBool
- toTruncated
