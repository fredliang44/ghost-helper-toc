ghost-helper-toc
================

Ghost Blog Handlebars Helper for Table of Contents


Installing
----------

Put the `toc.js` file into your current theme folder,
then change the file `ghost/index.js` like this:

```js
var express,
    ghost,
    parentApp,
    errors;

// add this line
require('./content/themes/yourtheme/toc')();

```


Usage
-----

```

{{toc}}

{{toc start="1" end="3"}}

```

Result:

```
<li><a href="#headline1">Headline H1</a></li>
<ul>
  <li><a href="#headline2">Headline H2</a></li>
  <ul>
    <li><a href="#headline3">Headline H3</a></li>
    <li><a href="#headline3">Headline H3</a></li>
  </ul>
  <li><a href="#headline2">Headline H2</a></li>
  <li><a href="#headline2">Headline H2</a></li>
  <li><a href="#headline2">Headline H2</a></li>
</ul>
```


License
-------

[MIT License](http://www.opensource.org/licenses/mit-license.php)

&copy; 2014 Béla Varga &lt;netzzwerg@gmail.com&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
