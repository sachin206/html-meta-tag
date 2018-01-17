# HTML Meta Tags
Meta Data:
	Meta data is information  about the html document.
	It does not displayed in page, it is machine parsable.
	
	There are different type of meta tag:
	<meta> tags always go inside the <head> element.

Meta data is always passed as name(name/http-equiv)/value(contnet) pairs.

The content attribute MUST be defined if the name or the http-equiv attribute is defined. If none of these are defined, the content attribute CANNOT be defined.

##  Some General Meta Tags
| Attribute | | Content(Possible Value of Meta Attribute) | Detail |   |
| --- | --- | --- | --- | --- |
|name | keywords | <keyword1, keyword2, keyword3….> | keywords tag is where you put all of the keywords you use in your site. ...It helps in SEO. |
|| description |<description of document………..> | this is used for defining document description (limit to 150 characters) |  |
|| viewport |__width:__ Sets the width of the layout viewport. In our case we set this to the “device-width” which overrides Apples default 960px.<br /> __initial-scale:__  Sets the initial zoom of the page AND the width of the layout viewport. We set this to 1 which is the default view, but you can easily increase this number (not recommended).<br /> __minimum-scale:__ Sets the minimum zoom level (i.e. how much the user can zoom out). This takes the control away from the user and something we never recommend.<br /> __maximum-scale:__ Sets the maximum zoom level (i.e. how much the user can zoom in). Again this is not recommended because it takes away control from the user.<br /> __height:__ Is supposed to set the height of the layout viewport. It is not supported anywhere…. so not really sure it’s included.<br /> __user-scalable:__ When set to no prevents the user from zooming. This is an abomination that MUST NOT be used. Even if you think you know what’s best for the user, you don’t, leave it alone.<br /> | this tag is used for controlling of rendering page. | |
|| generator |<program---name> for example worderpress, JOOMLA etc. | this tag is used for  page programming language which is used in creating this page/website |  |
|| robots |__INDEX:__ used for the search engine crawler to follow the links in that webpage,<br /> __FOLLOW:__ used for the search engine crawler to index webpage <br /> __NOFOLLOW:__ used for the search engine crawler NOT to follow the links in that webpage <br /> __NONINDEX:__ used for the search engine crawler NOT to index that webpage | Control the behavior of search engine crawling and indexing |  |
|| subject |your website's subject |  this is used for website subject|  |
|| application-name |name of application name. (only should be used if the website is used as an app) | this tag is used for company name  |  |
|| company |company name | this tag is used for company name  |  |
|| language |ES,EN,FR.... | this tag is used for defining language of html document |  |
|| author |name of the author | this tag is used for author of html document  |  |
|| revised |Revison Date of page for example Sunday, July 18th, 2010, 5:15 pm | used for revision of html document  |  |
|| rating| |  |  |
|| distribution | | |  |
|| coverage | | |  |
|| category | | |  |
|| directory | | |  |
|| identifier-URL | | |  |
|| owner | | |  |
|| revisit-after | | |  |
|| reply-to | | |  |
|| robots | | |  |
|| robots | | |  |
|| robots | | |  |
|| robots | | |  |
|| robots | | |  |
|| robots | | |  |
||  | |  |  |
|http-equiv | refresh | time & url on which page is redirected | Specifies a delay in seconds before the browser automatically reloads the document. Optionally, specifies an alternative URL to load, making this command useful for redirecting browsers to other pages. | |
|| x-ua-compatible | IE=edge,IE=11,IE=EmulateIE11,IE=10,IE=EmulateIE10, <br />IE=9,IE=EmulateIE9,IE=8,IE=EmulateIE8,IE=7,IE=EmulateIE7,IE=5 | this tag is used for IE browser to rendering the page in specific IE version. It should be used when page forced to be render in lowe version of IE. position of tag is just after head tag. |
|| Cache-Control | __default-src:__ the default policy for loading javascript, images, CSS, fonts, AJAX requests, etc <br /> __script-src:__ defines valid sources for javascript files __style-src:__ defines valid sources for css files<br /> __img-src:__ defines valid sources for images<br /> __connect-src:__ defines valid targets for to XMLHttpRequest (AJAX), WebSockets or EventSource. If a connection attempt is made to a host that's not allowed here, the browser will emulate a 400 error | meta-tag allows to reduce the risk of XSS attacks by allowing you to define where resources can be loaded from, preventing browsers from loading data from any other locations. This makes it harder for an attacker to inject malicious code to your site. |  |
|| Expires |Date on which this document will expire | The date and time after which the document should be considered expired. An illegal EXPIRES date, e.g. "0", is interpreted as "now". Setting EXPIRES to 0 may thus be used to force a modification check at each visit.
Web robots may delete expired documents from a search engine, or schedule a revisit. |  |
|| Pragma | |  |  |
|| Cache-Control | Allowed values = PUBLIC | PRIVATE | NO-CACHE | NO-STORE. |  |  |

##  Custom Meta Tags

Use custom meta tags to store data that you need in javascript, instead of hard-coding that data into your javascript.  I store my Google Analytics code in meta tags.  Here's some examples:

``` html
<meta name="google-analytics" content="1-AHFKALJ"/>
<meta name="disqus" content="abcdefg"/>
<meta name="uservoice" content="asdfasdf"/>
<meta name="mixpanel" content="asdfasdf"/>
```

## Company/Service Meta Tags

#### ClaimID

``` html
<meta name="microid" content="mailto+http:sha1:e6058ed7fca4a1921cq91d7f1f3b8736cd3cc1g7" />
```
    
#### Apple Meta Tags

``` html
<meta name="apple-mobile-web-app-capable" content="yes">
<meta content="yes" name="apple-touch-fullscreen" />
<meta name="apple-mobile-web-app-status-bar-style" content="black">
<meta name="format-detection" content="telephone=no">
<meta name="viewport" content="width = 320, initial-scale = 2.3, user-scalable = no">
```

#### Internet Explorer Meta Tags

``` html
<meta http-equiv="Page-Enter" content="RevealTrans(Duration=2.0,Transition=2)" />
<meta http-equiv="Page-Exit" content="RevealTrans(Duration=3.0,Transition=12)" />
<meta name="mssmarttagspreventparsing" content="true">
<meta http-equiv="X-UA-Compatible" content="chrome=1">
<meta name="msapplication-starturl" content="http://blog.reybango.com/about/"/>
<meta name="msapplication-window" content="width=800;height=600"/>
<meta name="msapplication-navbutton-color" content="red"/>
<meta name="application-name" content="Rey Bango Front-end Developer"/>
<meta name="msapplication-tooltip" content="Launch Rey Bango's Blog"/>
<meta name="msapplication-task" content="name=About;action-uri=/about/;icon-uri=/images/about.ico" />
<meta name="msapplication-task" content="name=The Big List;action-uri=/the-big-list-of-javascript-css-and-html-development-tools-libraries-projects-and-books/;icon-uri=/images/list_links.ico" />
<meta name="msapplication-task" content="name=jQuery Posts;action-uri=/category/jquery/;icon-uri=/images/jquery.ico" />
<meta name="msapplication-task" content="name=Start Developing;action-uri=/category/javascript/;icon-uri=/images/script.ico" />

```