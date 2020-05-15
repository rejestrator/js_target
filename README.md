# js_target
Set blank _target for specific links with javascript.

 ```js
 function externalLinks() {
  for(var c = document.getElementsByTagName("a"), a = 0;a < c.length;a++) {
    var b = c[a];
    b.getAttribute("href") && b.hostname !== location.hostname && (b.target = "_blank")
  } 
}; 
externalLinks();
```
