jquery-scroll-to
================

Animated auto scrolling

Features
--------
* aborts auto scrolling on user interaction

Usage
```
$(window).scrollTo(x, y, options);
$(window).scrollTo({top: x, left: y}, options);
$(window).scrollTo(element, options);
```

Example
-------

Create a back-to-top link
```
$(document).ready(function() {
  $('a.back-to-top').on('click', function(event) {
    $(window).scrollTo(0, 0);
  });
});
```


Options
-------
<table>
  <tr>
    <th>Name</th><th>Description</th><th>Default</th>
  </tr>
  <tr>
    <td>offset</td><td>an object containing top and left properties</td><td>{top: 0, left: 0}</td>
  </tr>
  <tr>
    <td colspan="3">jquery-animate options</td>
  </tr>
</table>


Rails
-----

To integrate jquery-scroll-to with rails add the jquery-benignware-rails gem to your application bundle

```
gem 'jquery-benignware-rails'
```

Require the javascript in your application.js
```
//= require benignware/jquery.scroll-to.js
```
