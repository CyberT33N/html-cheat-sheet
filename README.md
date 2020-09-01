# HTML Cheat Sheet
HTML Cheat Sheet with the most needed stuff..
<br />
<br />
<br />
<br />

# Meta List
- https://gist.github.com/lancejpollard/1978404



# Default Layout
```html
<!DOCTYPE html>
<html lang="en">
<head>

  <!-- redirect to different page when user got no javascript -->
  <noscript><meta http-equiv="refresh" content="0; url=./nojs/index.html" /></noscript>

<!-- set description and title for SEO-->
<meta
name="description"
content="Dennis Demand | CyberT33N (Software Developer & WEB Designer)
► Node.js ● Scrap/Crawl ● Automate ● Electron.js ● WEB Design ◄"/>
<title>Resume - Dennis Demand (Software Developer & WEB Designer)</title>
<meta property="image" content="https://resume.cybert33n.com/img/logo.webp"/>
<meta name="keywords" content="Window, Linux, MAC, Node.js, Javascript, CSS, HTML, SVG, PHP, Regex, Bash, CMD, Electron.js, Automation, Scrap/Crawl, Puppeteer, Webdriver.io, Cheerio.js, Chromium, Anime.js, Tippy.js, jQuery, Chromium Extensions, Express.js, Socket.io, REST API, VPS, Apache, Heroku, Digital Ocean, Google Cloud, Domain, Web/Virtualmin, SSL, FFmpeg, SMTP, XAMPP, PhpMyAdmin, MySQL, MongoDB, Opencart, Wordpress, Discord API, Google Sheet API, Google Drive API, YouTube API, Dropbox API, OneDrive API, Box, Virtualbox, VeraCrypt (GUI & CLI), VPN/Proxy/Socks5 (OpenVPN, NordVPN), Adobe Photoshop, Adobe After Effects, Adobe InDesign, Adobe Illustrator"/>
<meta name="subject" content="Resume"/>
<meta name="copyright"content="Dennis Demand (CyberT33N)"/>
<meta name="language" content="EN"/>
<meta name="robots" content="index,follow" />
<meta name="Classification" content="Business"/>
<meta name="author" content="Dennis Demand (CyberT33N)"/>
<meta name="designer" content="Dennis Demand (CyberT33N)"/>
<meta name="owner" content="Dennis Demand (CyberT33N)"/>
<meta name="url" content="https://resume.cybert33n.com"/>
<meta name="identifier-URL" content="https://resume.cybert33n.com"/>
<meta name="coverage" content="Worldwide"/>
<meta name="distribution" content="Global"/>
<meta name="rating" content="General"/>














<!-- facebook-->
<meta property="og:title" content="Resume - Dennis Demand (Software Developer & WEB Designer)"/>
<meta property="og:image" content="https://resume.cybert33n.com/img/logo.webp"/>
<meta property="og:description" content="Dennis Demand | CyberT33N (Software Developer & WEB Designer)
► Node.js ● Scrap/Crawl ● Automate ● Electron.js ● WEB Design ◄"/>
<meta property="og:url" content="https://resume.cybert33n.com"/>
<meta name="og:type" content="resume"/>
<meta name="og:site_name" content="CyberT33N Resume"/>

<!--
<meta name="og:email" content="me@example.com"/>
<meta name="og:phone_number" content="650-123-4567"/>
<meta name="og:fax_number" content="+1-415-123-4567"/>

<meta name="og:latitude" content="37.416343"/>
<meta name="og:longitude" content="-122.153013"/>
<meta name="og:street-address" content="1601 S California Ave"/>
<meta name="og:locality" content="Palo Alto"/>
-->
<meta name="og:locality" content="Duisburg"/>
<meta name="og:region" content="NRW"/>
<meta name="og:postal-code" content="47279"/>
<meta name="og:country-name" content="Germany"/>




<!-- twitter-->
<meta name="twitter:title" content="Resume - Dennis Demand (Software Developer & WEB Designer)"/>
<meta name="twitter:description" content="Dennis Demand | CyberT33N (Software Developer & WEB Designer)
► Node.js ● Scrap/Crawl ● Automate ● Electron.js ● WEB Design ◄"/>
<meta name="twitter:image" content="https://resume.cybert33n.com/img/logo.webp"/>
<meta name="twitter:card" content="summary_large_image"/>



<!--  Non-Essential, But Recommended -->
<meta property="og:site_name" content="Resume - Dennis Demand (Software Developer & WEB Designer)"/>


<!--  Non-Essential, But Required for Analytics
<meta property="fb:app_id" content="your_app_id" />
<meta name="twitter:site" content="@website-username"/>
-->















  <!-- set viewport for responsive and enable utf8-->
  <meta name="viewport" content="width=device-width, height=device-height, initial-scale=1, minimum-scale=1, maximum-scale=1, user-scalable=no, minimal-ui"/>
  <meta charset="UTF-8"/>

   <!-- prevent cache -->
  <meta http-equiv='cache-control' content='no-cache, no-store, must-revalidate'/>
  <meta http-equiv='expires' content='0'/>
  <meta http-equiv='pragma' content='no-cache'/>


  <!-- run fullscreen on web apps -->
  <meta name="apple-mobile-web-app-capable" content="yes"/>
  <meta name="mobile-web-app-capable" content="yes"/>

  <!-- Style user adress bar -->
 <meta name="theme-color" content="#5c5c5c"/>


  <!-- favicons -->
<link rel="apple-touch-icon" href="favicon.ico" type="image/x-icon" />
<link rel="shortcut icon" href="favicon.ico" type="image/x-icon" />



 <!-- your stlyesheets here -->
<link rel="stylesheet" href="css/bootstrap.min.css"/>
<link rel="stylesheet" href="css/style.css"/>

</head>






<body>
 
 
 <!-- your scripts here - if possible use defer & async -->
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
