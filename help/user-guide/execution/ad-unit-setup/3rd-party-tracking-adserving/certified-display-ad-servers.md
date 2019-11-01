---
edit-last: 17
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
ldc-disable: 0
ldc-disable-comm: 0
pubDate: Wed, 10 Jun 2015 17:53:02 +0000
dc-creator: hthomas@adobe.com
guid: https://education.tubemogul.com/?page_id=4033
isPermaLink: false
description: 
postId: 4033
postDate: 2015-06-10 09:53:02
postDateGmt: 2015-06-10 17:53:02
commentStatus: open
pingStatus: open
postName: certified-display-ad-servers
status: publish
postParent: 1821
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Certified Display Ad Servers {#certified-display-ad-servers}

TubeMogul currently accepts the following certified display ad servers. Please review the below to ensure delivery and minimal reporting discrepancies,&nbsp;and make sure your 3rd party ad tags are&nbsp;SSL compliant (https).

![DFA](assets/dfa.jpg)

The platform supports iFrame & javascript tags only. No IMG or HREF. 

![0_jivoxlogosmall](assets/0-jivoxlogosmall.gif)

The platform supports all Desktop ad sizes, including rich media expandable banners and mobile in-app.

![Sizmek](assets/sizmek-300x300.png)

The platform supports Desktop and 300x250 mobile web units only. No mobile in-app.

![medialets](assets/medialets-150x135.png)

The platform supports javascript and IMG tags.
The tags do require a small formatting change before adding into the platform. The tag below shows the additions highlighted in **YELLOW.** 

```

<pre><<script type="text/javascript"> &nbsp;(function(s,n,u,o,i){ for(i in o)o.hasOwnProperty(i)&&(u+='&'+i+'='+encodeURIComponent(o[i]));document.write('<script src= <span style="background-color: yellow;"><strong>\</strong></span>"'+(location.protocol=='https:'?s+u:n+u+decodeURI('<span style="background-color: yellow;"><strong>\</strong></span>" onerror=<span style="background-color: yellow;"><strong>\</strong></span>"document.write(%27<script src=%5c%27')+s+u+decodeURI('%5c%27><%27+%27/script>%27)'))+'<span style="background-color: yellow;"><strong>\</strong></span>"><'+'/script>'); }('https://s-cdn-tag.medialytics.com','https://tag.medialytics.com','/tag?format=dw',{ tagID: "sb376d0055b3a4e13aeeebe43a957157d", click: "${TM_CLICK_URL}$$_DESTINATION_URL_$$", ls: true, imppx: "" })); </script> <noscript> <a target="_blank" href="https://clk.medialytics.com/href?0.type=i&0.key=MMAdClickthrough&tagID=sb376d0055b3a4e13aeeebe43a957157d&impunique=${TM_RANDOM}"> <img src="https://c.medialytics.com /creative?type=s&tagID=sb376d0055b3a4e13aeeebe43a957157d&impunique=${TM_RANDOM}" width="300" height="250"/> </a> </noscript></pre>

```

![conversant](assets/conversant.png)

The platform Supports iFrame & javascript tags for desktop and mobile web units only. No IMG, HREF, or mobile in-app tags.

Conversant tags also require users to manually insert macros for tracking, see below for example code with inserted macros highlighted in **YELLOW**:   

```

<pre><iframe src="https://<a href="https://altfarm.mediaplex.com/ad/fm/18630-145298-44091-1?mpt=" target="_blank">altfarm.mediaplex.<wbr>com/ad/fm/18630-145298-44091-<wbr>1?mpt=</a><span style="background-color: yellow;">${TM_RANDOM}</span>&mpvc=<span style="background-color: yellow;">${TM_<wbr>CLICK_URL_URLENC}</span>" width=300 height=250 marginwidth=0 marginheight=0 hspace=0 vspace=0 frameborder=0 scrolling=no bordercolor="#000000">
<br><script type="text/javascript" src="https://<a href="https://altfarm.mediaplex.com/ad/!js/18630-145298-44091-1?mpt=$%7BTM_RANDOM%7D&mpvc=" target="_blank">altfarm.mediaplex.<wbr>com/ad/!js/18630-145298-44091-<wbr>1?mpt=${TM_RANDOM}&mpvc=</a><span style="background-color: yellow;">${TM_<wbr>CLICK_URL_URLENC}</span>">
<br></script>
<br><noscript>
<br><a href="<span style="background-color: yellow;">${TM_CLICK_URL_URLENC}</span>ht<wbr>tp://<a href="https://altfarm.mediaplex.com/ad/nc/18630-145298-44091-1?mpt=" target="_blank">altfarm.mediaplex.com/ad/<wbr>nc/18630-145298-44091-1?mpt=</a><span style="background-color: yellow;">${<wbr>TM_RANDOM}</span>">
<br><img src="https://<a href="https://altfarm.mediaplex.com/ad/nb/18630-145298-44091-1?mpt=" target="_blank">altfarm.mediaplex.<wbr>com/ad/nb/18630-145298-44091-<wbr>1?mpt=</a><span style="background-color: yellow;">${<wbr>TM_RANDOM}</span>"alt="Click Here" border="0">
<br></a>
<br></noscript>
<br></iframe></pre>

```

![flashtalking-logo1](assets/flashtalking-logo1.jpg)

The platform supports iFrame & javascript tags.
FlashTalking tags also require manual insertion of macros for click tracking, see below for example code with inserted macros highlighted in **YELLOW**:   

```

<noscript> 
<a href=" `**${TM_CLICK_URL_URLENC}**` [ht`<wbr>`tp://servedby.flashtalking.`<wbr>`com/click/8/57258;1799696;0;`<wbr>`209;0/?ft_width=300&ft_height=`<wbr>`250&url=9678632](https://servedby.flashtalking.com/click/8/57258;1799696;0;209;0/?ft_width=300&ft_height=250&url=9678632)" target="_blank"> 
<img border="0" src=" [https://servedby.`<wbr>`flashtalking.com/imp/8/57258;`<wbr>`1799696;205;gif;Tubemogul;`<wbr>`300x250HTML5StandardwClickExte`<wbr>`nsion/](https://servedby.flashtalking.com/imp/8/57258;1799696;205;gif;Tubemogul;300x250HTML5StandardwClickExtension/)?"></a> 
</noscript> 
<script language="Javascript1.1" type="text/javascript"> 
var ftClick = " `**${TM_CLICK_URL_URLENC}**";` 
var ftExpTrack_1799696 = ""; 
var ftX = ""; 
var ftY = ""; 
var ftZ = ""; 
var ftOBA = 1; 
var ftContent = ""; 
var ftCustom = ""; 
var ftSection = " ${TM_SITE_ID_NUM}"; 
var ftID = function(){for(var e=["${USER_ID}"],a=e.length,r= `<wbr>`"";a--;)if(e[a]&&!RegExp("[^a- `<wbr>`z0-9q-]".replace(/q/g, `<wbr>`decodeURIComponent("%5"+"C")), `<wbr>`"i").test(e[a])){r=e[a];break} `<wbr>`return r}();; 
var ft300x250_OOBclickTrack = ""; 
var ftRandom = Math.random()&#42;1000000; 
var ftBuildTag1 = "<scr"; 
var ftBuildTag2 = "</"; 
var ftClick_1799696 = ftClick; 
if(typeof(ft_referrer)==" `<wbr>`undefined"){var ft_referrer=(function(){var r="";if(window==top){r=window. `<wbr>`location.href;}else{try{r= `<wbr>`window.parent.location.href;} `<wbr>`catch(e){}r=(r)?r:document. `<wbr>`referrer;}while( `<wbr>`encodeURIComponent(r).length> `<wbr>`1000){r=r.substring(0,r. `<wbr>`length-1);}return r;}());} 
var ftDomain = (window==top)?"":(function(){ `<wbr>`var d=document.referrer,h=(d)?d. `<wbr>`match("(?::q/q/)+([qw-]+(q.[ `<wbr>`qw-]+)+)(q/)?".replace(/q/g, `<wbr>`decodeURIComponent("%"+"5C"))) `<wbr>`[1]:"";return (h&&h!=location.host)?"&ft_ `<wbr>`ifb=1&ft_domain="+ `<wbr>`encodeURIComponent(h):"";}()); 
var ftTag = ftBuildTag1 + 'ipt language="javascript1.1" type="text/javascript" '; 
ftTag += 'src=" [https://servedby.`<wbr>`flashtalking.com/imp/8/57258;`<wbr>`1799696;201;js;Tubemogul;`<wbr>`300x250HTML5StandardwClickExte`<wbr>`nsion/?ftx='+ftX+'&fty='+ftY+'`<wbr>`&ftadz='+ftZ+'&ftscw='+`<wbr>`ftContent+'&ft_custom='+`<wbr>`ftCustom+'&ft_section='+`<wbr>`ftSection+'&ft_id='+ftID+'&`<wbr>`ftOBA='+ftOBA+ftDomain+'&ft_`<wbr>`referrer='+encodeURIComponent(`<wbr>`ft_referrer)+'&cachebuster='+`<wbr>`ftRandom+](https://servedby.flashtalking.com/imp/8/57258;1799696;201;js;Tubemogul;300x250HTML5StandardwClickExtension/?ftx=%27+ftX+%27&fty=%27+ftY+%27&ftadz=%27+ftZ+%27&ftscw=%27+ftContent+%27&ft_custom=%27+ftCustom+%27&ft_section=%27+ftSection+%27&ft_id=%27+ftID+%27&ftOBA=%27+ftOBA+ftDomain+%27&ft_referrer=%27+encodeURIComponent(ft_referrer)+%27&cachebuster=%27+ftRandom+)'" id="ftscript_300x250" name="ftscript_300x250"'; 
ftTag += '>' + ftBuildTag2 + 'script>'; 
document.write(ftTag); 
</script>

```