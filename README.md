AntiModerate
===

The progressive image loading library for great good!

---


Reduce loading time of page to less than a second on slow connections by loading and rendering nicely blurred micro images on the page while loading full sized images in background which replace as they finish.

Has a nice blur effect thanks to [StackBlur](https://github.com/flozz/StackBlur/) so you have a good looking page while it is loading.

Library is space optimized, with gzip it is less than 2kb.


![Example](http://i.imgur.com/fkgiPNe.png)

##Installation

You can install this using `bower` or `npm`:

```
  bower install antimoderate
```
```
  npm install antimoderate --save
```

##Example


```html
<img src="1.jpg" id="picture" style="width:200px; height:200px;" data-antimoderate-idata="data:image/jpg;base64, /9j/4AAQSkZJRgABAQEASABIAAD//gATQ3JlYXRlZCB3aXRoIEdJTVD/2wBDAAoHBwgHBgoICAgLCgoLDhgQDg0NDh0VFhEYIx8lJCIfIiEmKzcvJik0KSEiMEExNDk7Pj4+JS5ESUM8SDc9Pjv/2wBDAQoLCw4NDhwQEBw7KCIoOzs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozs7Ozv/wgARCAAlACgDAREAAhEBAxEB/8QAGQAAAgMBAAAAAAAAAAAAAAAAAwQCBQYB/8QAGAEBAQEBAQAAAAAAAAAAAAAAAAEDAgT/2gAMAwEAAhADEAAAAeyqgi0iYKg56Gw9ZfX4JRCq+VfjV3TGxgdZhFKcNJyNWUpYOajl/8QAHxAAAgICAgMBAAAAAAAAAAAAAQIAAwQTEjERISQj/9oACAEBAAEFApdZrVbrEMHcYeLba9og7mXbqV8rYtF/KDuZLfWCFisDMdi1XGZdf1mv1UnrFH4//8QAHREAAgIBBQAAAAAAAAAAAAAAAQMAESACITAxMv/aAAgBAwEBPwHJfqMXfeANGMcdW3L/AP/EABsRAAEFAQEAAAAAAAAAAAAAAAECEBEgMQAD/9oACAECAQE/AaHGXnJXGMcdPnBljlTlT3//xAAfEAABAwQDAQAAAAAAAAAAAAABAAIxEBEhQRITgSD/2gAIAQEABj8CWJMIdkHdBRrrD1C+vhuLklcW+ri+avvrAq0mj8qVMJq//8QAIhAAAgIBBAEFAAAAAAAAAAAAAAERITFBUWFxkbHB0eHx/9oACAEBAAE/IYI5QxhRpOOFiQvmILCNOAmRSllbCQleyBSOkLwNsFFSdlOjS9xKdkD062BtQ2+BNCcmRf7Ox2uHjg/IJ29AqZw/c//aAAwDAQACAAMAAAAQEOE8lCmMc38Gf//EABsRAQEBAAIDAAAAAAAAAAAAAAERABAgITGx/9oACAEDAQE/ENdE99HAzAa5PnSA4GPBryMeTt//xAAcEQACAwEAAwAAAAAAAAAAAAAAARARMSEgQbH/2gAIAQIBAT8QKLTyNI7Lnr2+xpDVqhdjRo0irU7eCOk0f//EACMQAQACAQIGAwEAAAAAAAAAAAEAESExQRBRYXGRsYGh8OH/2gAIAQEAAT8QY1kLJt1lp1AlBtacDwD3w6OoWqqKZIsZhNz5cHxL3DohlQbSiDWOaXAsbyekoCxhs/3PFvcIXeoGOCjP2sHK5vNc+ZaAjvRMyjwvOqX9Q/BMZpfgOs06dPzWbBYd0W5aw07p/9k=">
```

```html
<script src="antimoderate.js"></script>
<script>
    var img = document.getElementById('picture');

    AntiModerate.process(img, img.getAttribute("data-antimoderate-idata"));
</script>
```


##License

###AntiModerate

~~~
Copyright (c) 2016 Jett LaRue

Do whatever with it.

~~~


###StackBlur Algorithm


~~~
Copyright (c) 2010 Mario Klingemann

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.
~~~
