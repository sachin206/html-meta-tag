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
|| author |<author name....> | this tag is used for author of html document  |  |
|| revised |Revison Date Sunday, July 18th, 2010, 5:15 pm | used for revision of html document  |  |
|| viewport |[width=device-width, initial-scale=1, shrink-to-fit=no],[width=500, initial-scale=1],[width=...,initial-scale=...,maximum-scale=...,user-scalable=...,minimum-scale=....] | this tag is used for controlling of rendering page. | |
|| generator |<program---name> for example worderpress, JOOMLA etc. | this tag is used for  page programming language which is used in creating this page/website |  |
|| subject |your website's subject |  this is used for website subject|  |
|| company |company name | this tag is used for company name  |  |
|| language |ES,EN,FR.... | this tag is used for defining language of html document |  |
|| robots |__INDEX:__ used for the search engine crawler to follow the links in that webpage,<br /> __FOLLOW:__ used for the search engine crawler to index webpage <br /> __NOFOLLOW:__ used for the search engine crawler NOT to follow the links in that webpage <br /> __NONINDEX:__ used for the search engine crawler NOT to index that webpage | Control the behavior of search engine crawling and indexing |  |
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
|http-equiv | refresh |  |  |
|| Expires |index,follow |  |  |
|| Pragma | |  |  |
|| Cache-Control | |  |  |

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