# ot
ot mean object template

```
var obj;
var temp='<img src="{download_url}" alt="{name}">'
document.body.innerHTML=ot(temp,obj,def)
```
```
var re=/\{[\w\.]*\}/
var deep =(tag)=> (tag.match(/\./g)||[]).length

obj.deep0.deep1.deep2

obj[deep0][deep1][deep2]

check deep
```
```
// First, checks if it isn't implemented yet.
if (!String.prototype.format) {
  String.prototype.format = function() {
    var args = arguments;
    return this.replace(/{(\d+)}/g, function(match, number) { 
      return typeof args[number] != 'undefined'
        ? args[number]
        : match
      ;
    });
  };
}
```


```

var o={x:0,y:0,v:'N',c:'A'};
[o].map(d=>`${d.x}${d.y}${v}`)

```













