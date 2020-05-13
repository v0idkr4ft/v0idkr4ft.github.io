---
layout: "post"
title: "CodePen.IO"
date: "2020-05-13 18:30"
tags: [codepen, code, css, html]
---

## webkit animation ##

<div class="wrapz" style="margin:0 auto;">
  <div class="wobz">
    <img class="rotate-element" src="https://v0idkr4ft.com/assets/img/spiral2.png">
  </div>
  <div class="fcspnspn">
    <div class="hovertate">
      <div class="fwobz">
        <a href="forum.v0idkr4ft.com" target="_blank" class="link"><img src="https://v0idkr4ft.com/assets/img/fcpng.png"></a>
      </div>
    </div>
  </div>
</div>

[CodePen.Io][e60a62ec] *codes & fiddles*-


Html
```
<body bgcolor="black">
<div class="wrapz">
  <div class="wobz">
  <img class="rotate-element" src="https://v0idkr4ft.com/assets/img/spiral2.png">
  </div>
  <div class="fcspnspn">
    <div class="hovertate">
      <div class="fwobz">
      <a href="forum.v0idkr4ft.com" target="_blank" class="link"><img src="https://v0idkr4ft.com/assets/img/fcpng.png"></a>
      </div>
    </div>
        </div>
</div>
</body>
```

CSS
{% highlight css %}
@-webkit-keyframes infiniteRotate {    
     0% { -webkit-transform: rotate(0deg); }
     100% { -webkit-transform: rotate(360deg); }
}
/* Standard syntax */
@keyframes infinite-rotate {  
     0% { -webkit-transform: rotate(0deg); }
     100% { -webkit-transform: rotate(360deg); }
}
.rotate-element {
align: center;
width: 200px;
height: 200px;
-webkit-animation: infiniteRotate 1s linear infinite; /* Safari */
animation: infiniteRotate 1s linear infinite;
}

@-webkit-keyframes wubz {    
      0% { -webkit-transform:
scale3d(1, 1, 1); }
     40% { -webkit-transform: scale3d(0.7, 0.9, 1); }
     75% { -webkit-transform: scale3d(1.3, 1.1, 1); }
     100% { -webkit-transform: scale3d(1, 1, 0.3); }
}
.wobz {
-webkit-border-radius: 50%;
      border-radius: 50%;

}
.wobz:hover {
-webkit-animation: wubz 3s ease infinite alternate;
}

.wrapz {
position: relative;
display: table;
margin:0 auto;
}
.fcspnspn {
z-index: 20;
width: 75%;
/* height: 100%; */
/* margin-left: 15%; */
/* vertical-align: middle; */
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%,-50%);
}
.hovertate {

}
.hovertate:hover {

-webkit-animation: infiniteRotate 1s linear infinite; /* Safari */
animation: infiniteRotate 1s linear infinite;
}

@-webkit-keyframes fwubz {    
      0% { -webkit-transform:
scale3d(1, 1, 1); }
     40% { -webkit-transform: scale3d(0.1, 0.2, .4); }
     75% { -webkit-transform: scale3d(1.5, 1.5, 1.5); }
     100% { -webkit-transform: scale3d(.7, .5, 0.3); }
}
.twobz {
-webkit-border-radius: 50%;
      border-radius: 50%;

}
.fwobz:hover {
-webkit-animation: fwubz 3s ease infinite alternate;
}
{% endhighlight %}

  [e60a62ec]: https://codepen.io/v0idkr4ft "Codes & Fiddles / animation snippets."
