```javascript
window.jsopen = function(path) {
  var el = document.createElement('script');
  if(path.indexOf('http') == 0) {
    el.src = path;
  } else {
    el.src = 'http://cdnjs.cloudflare.com/ajax/libs/'+path;
  }
  document.head.appendChild(el);
}
```

 Paste the following script to Chrome devTools
 and pass the missing part of the needed path as the function argument

 Example: insert jQuery cdnjs url:

```javascript
window.jsopen('jquery/2.1.3/jquery.min.js')
```
Voila! Now you can use the library in your Chrome Dev console!
