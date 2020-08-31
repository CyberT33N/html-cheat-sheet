# HTML Cheat Sheet
HTML Cheat Sheet with the most needed stuff..
<br />
<br />
<br />
<br />



# Default Layout
```html
<!DOCTYPE html>
<html lang="en">
<head>
<noscript><meta http-equiv="refresh" content="0; url=./nojs/index.html" /></noscript>
<meta
name="description"
content="Dennis Demand | CyberT33N (Software Developer & WEB Designer)
► Node.js ● Scrap/Crawl ● Automate ● Electron.js ● WEB Design ◄">
<title>Resume - Dennis Demand (Software Developer & WEB Designer)</title>
<meta name="viewport" content="width=device-width, height=device-height, initial-scale=1, minimum-scale=1, maximum-scale=1, user-scalable=no">
<meta charset="UTF-8">
<meta http-equiv='cache-control' content='no-cache, no-store, must-revalidate'>
<meta http-equiv='expires' content='0'>
<meta http-equiv='pragma' content='no-cache'>

  <!-- run fullscreen -->
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="mobile-web-app-capable" content="yes">

  <!-- Style user adress bar -->
 <meta name="theme-color" content="#5c5c5c"/>


 
<link rel="stylesheet" href="css/style.css"/>

</head>






<body>
 
 

<script src="js/scripts.js" defer> </script>
</body>
</html>
 
 

```


<br />
<br />


 _____________________________________________________
 _____________________________________________________


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
