# ot
ot mean object template

```
var obj;
var temp='<img src="{download_url}" alt="{name}">'
document.body.innerHTML=ot(temp,obj)
```
```
var re=/\{[\w\.]*\}/
var deep =(tag)=> (tag.match(/\./g)||[]).length

obj.deep0.deep1.deep2

obj[deep0][deep1][deep2]

check deep
```
