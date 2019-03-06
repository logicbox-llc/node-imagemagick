# node-imagemagick with composite func

[Imagemagick](http://www.imagemagick.org/) module for [Node](http://nodejs.org/).

You can install this module using npm:

    npm install @logicbox-llc/imagemagick

Requires imagemagick CLI tools to be installed. There are numerous ways to install them. For instance, if you're on OS X you can use [Homebrew](http://mxcl.github.com/homebrew/): `brew install imagemagick`.

## Example

```javascript
var im = require('@logicbox-llc/imagemagick');
im.readMetadata('kittens.jpg', function(err, metadata){
  if (err) throw err;
  console.log('Shot at '+metadata.exif.dateTimeOriginal);
})
// -> Shot at Tue, 06 Feb 2007 21:13:54 GMT
```

...

## License (MIT)

Copyright (c) 2010-2012 Rasmus Andersson <http://hunch.se/>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
