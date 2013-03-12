jquery-imagefallback
====================

Encapsulate fallback behavior when images fail to load. Works with Zepto.js as well. :)

Call `$('.foo').fallback` on an image selector to fallback to another image if the
main image fails to load.

Usage
=====

There are two ways to use it.

1. Specify a fallback image URL
```javascript
$('img.photo').fallback('http://google.com/fallback.jpg');
```

2. Specify a callback function: 
```javascript
    $('.photo-container > img').fallback(function () {
        $('.photo-container').hide();
    }).attr('src', 'http://my.photosite.com/image1.jpg');
```
