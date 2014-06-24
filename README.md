DOMstagram
==========

Collection of bookmarklets which will eventually be built in to a Chrome extension to aid with styling up ajax web apps

[Refreshh CSS](javascript:(function()%7Bvar h,a,f%3Ba%3Ddocument.getElementsByTagName(%27link%27)%3Bfor(h%3D0%3Bh<a.length%3Bh%2B%2B)%7Bf%3Da%5Bh%5D%3Bif(f.rel.toLowerCase().match(/stylesheet/)%26%26f.href)%7Bvar g%3Df.href.replace(/(%26%7C%5C%3F)forceReload%3D%5Cd%2B/,%27%27)%3Bf.href%3Dg%2B(g.match(/%5C%3F/)%3F%27%26%27:%27%3F%27)%2B%27forceReload%3D%27%2B(new Date().valueOf())%7D%7D%7D)())

[Snapshot DOM](javascript:localStorage.setItem("snapshot", document.documentElement.innerHTML))

[Restore DOM](javascript:document.documentElement.innerHTML = localStorage.getItem("snapshot")
