# angular-loading-intro
Will show loading intro before app init 


add this lines into <head> element of index.html or first page loaded into browser

<style>.center{position:absolute;top:40%;left:30%;width:40%}.center div:first-child{font-family:Verdana,serif;font-size:16px;color:#b2b2b2;display:block;margin:0 auto;text-align:center;padding-bottom:10px}.bar{width:100%;height:5px;background-color:#b4dfaa;display:block;position:relative;overflow:hidden}.bar div{position:absolute;left:0;top:0;bottom:0;height:5px;background-color:#59b947}.line1{animation:progress-linear-scale 2s infinite,progress-linear 2s infinite;width:250px}.line2{animation:progress-linear-scale 4s infinite,progress-linear2 4s infinite;width:250px}@keyframes progress-linear-scale{0%{transform:scaleX(.3);animation-timing-function:linear}36.6%{transform:scaleX(.6);animation-timing-function:cubic-bezier(.3,.5,.7,1)}69.15%{transform:scaleX(.8);animation-timing-function:cubic-bezier(.3,.5,.7,1)}100%{transform:scaleX(1)}}@keyframes progress-linear{0%{left:-50%;animation-timing-function:linear}100%{left:150%;animation-timing-function:linear}}@keyframes progress-linear2{0%{left:-100%;animation-timing-function:linear}100%{left:150%;animation-timing-function:linear}}</style>


add this line inside <app> element 
or inside <ion-app> element 
* this element will be replaced as the app will init by angular framework


<div images="['img/login-bg-image.jpg']">
      <div class="center"><div>Loading...</div><div class="bar"><div class="line1"></div><div class="line2"></div></div></div>
    </div>
    
