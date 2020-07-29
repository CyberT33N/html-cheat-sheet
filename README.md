# HTML Cheat Sheet
HTML Cheat Sheet with the most needed stuff..
<br />
<br />
<br />
<br />



## Stop reload page on empty href
```html
<!--  method 1 -->
<a href="javascript:void(0)" onclick="window.open('img/upwork/jobs/job1.jpg', '_blank');">view contract</a>

<!--  method 2 -->
<a href="javascript:;" onclick="window.open('img/upwork/jobs/job1.jpg', '_blank');">view contract</a>
```  

## Open link new window
```html
<a href="javascript:void(0)" onclick="window.open('img/upwork/jobs/job1.jpg', '_blank', 'location=yes,height=$(window).height(),width=$(window).width(),scrollbars=yes,status=yes');">view contract</a>
``` 

<br />
<br />


 _____________________________________________________
 _____________________________________________________


<br />
<br />


## Hide placeholder on input focus
```html
<input 
type="text" 
placeholder="enter your text" 
onfocus="this.placeholder = ''"
onblur="this.placeholder = 'enter your text'" />
``` 

<br />
<br />


 _____________________________________________________
 _____________________________________________________


<br />
<br />

## Load .js files faster
```html
<!-- https://www.youtube.com/watch?v=BMuFBYw91UQ
If you specify both, async takes precedence on modern browsers, while older browsers that support defer but not async will fallback to defer.
-->
<script src="https://www.google.com/recaptcha/api.js" async defer></script>
``` 

<br />
<br />


 _____________________________________________________
 _____________________________________________________


<br />
<br />
