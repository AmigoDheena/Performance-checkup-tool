# Performance-checkup-tool
Performance Checkup Tool is a Chrome Bookmarklet script that is used to check your Website performance in GooglePageSpeed and GTmetrix by a single click

Just add this into the URL section of a new bookmark:

### Google PageSpeed Insight + GTmetrix
```javascript
javascript:(function(){var url=window.location.href;var pagespeed="https://developers.google.com/speed/pagespeed/insights/?url="+url;window.open(pagespeed);var n='https://gtmetrix.com/analyze.html?bm',t={url:window.location.href},i=function(n,t){var f=window.open(n),i=f.document.createElement('form'),u,r;i.setAttribute('method','post'),i.setAttribute('action',n);for(u in t)t.hasOwnProperty(u)&&(r=document.createElement('input'),r.setAttribute('type','hidden'),r.setAttribute('name',u),r.setAttribute('value',t[u]),i.appendChild(r));f.document.body.appendChild(i),i.submit()};i(n,t)})();
```

### Google PageSpeed Insight
```javascript
javascript:(function(){var url=window.location.href;var pagespeed="https://developers.google.com/speed/pagespeed/insights/?url="+url;window.open(pagespeed);})();
```

### GTmetrix
```javascript
javascript:(function(){var n='https://gtmetrix.com/analyze.html?bm',t={url:window.location.href},i=function(n,t){var f=window.open(n),i=f.document.createElement('form'),u,r;i.setAttribute('method','post'),i.setAttribute('action',n);for(u in t)t.hasOwnProperty(u)&&(r=document.createElement('input'),r.setAttribute('type','hidden'),r.setAttribute('name',u),r.setAttribute('value',t[u]),i.appendChild(r));f.document.body.appendChild(i),i.submit()};i(n,t)})();
```