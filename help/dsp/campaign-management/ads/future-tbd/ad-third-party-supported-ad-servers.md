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

---
title: Supported Third-party Ad Servers
description: Supported Third-party Ad Servers
---
# Supported Third-party Ad Servers

Advertising Cloud DSP currently accepts the following certified display ad servers.

<!--
![DFA](/help/dsp/assets/dfa.jpg)
-->

Supported: iFrame & JavaScript tags only

<!--
![0_jivoxlogosmall](/help/dsp/assets/0-jivoxlogosmall.gif)
-->

Supported: all desktop ad sizes, including rich media expandable banners and mobile in-app

<!--
![Sizmek](/help/dsp/assets/sizmek-300x300.png)
-->

Supported: Desktop and 300x250 mobile web units only

<!--
![medialets](/help/dsp/assets/medialets-150x135.png)
-->

Supported: JavaScript and IMG tags

>[!NOTE]
>
>For each Medialets tag, you must manually insert a backslash (`\`) in several places. The following example tag shows the required backslashes highlighted in yellow. 

<!--
![Example tag for Medialets](/help/dsp/assets/medailets_example_tag.png)
-->

<!-- Replace screen shot image with code block with appropriate highlighting once code highlighting is available. -->

<!--

```
<pre><<script type="text/javascript">  (function(s,n,u,o,i){ for(i in o)o.hasOwnProperty(i)&&(u+='&'+i+'='+encodeURIComponent(o[i]));document.write('<script src= <span style="background-color: yellow;"><strong>\</strong></span>"'+(location.protocol=='https:'?s+u:n+u+decodeURI('<span style="background-color: yellow;"><strong>\</strong></span>" onerror=<span style="background-color: yellow;"><strong>\</strong></span>"document.write(%27<script src=%5c%27')+s+u+decodeURI('%5c%27><%27+%27/script>%27)'))+'<span style="background-color: yellow;"><strong>\</strong></span>"><'+'/script>'); }('https://s-cdn-tag.medialytics.com','https://tag.medialytics.com','/tag?format=dw',{ tagID: "sb376d0055b3a4e13aeeebe43a957157d", click: "${TM_CLICK_URL}$$_DESTINATION_URL_$$", ls: true, imppx: "" })); </script> <noscript> <a target="_blank" href="https://clk.medialytics.com/href?0.type=i&0.key=MMAdClickthrough&tagID=sb376d0055b3a4e13aeeebe43a957157d&impunique=${TM_RANDOM}"> <img src="https://c.medialytics.com /creative?type=s&tagID=sb376d0055b3a4e13aeeebe43a957157d&impunique=${TM_RANDOM}" width="300" height="250"/> </a> </noscript></pre>
```

-->

<!--
![conversant](/help/dsp/assets/conversant.png)
-->

Supported: iFrame & JavaScript tags for desktop and mobile web units only

>[!NOTE]
>
>For each Conversant tag, you must manually insert the tracking macros `${TM_RANDOM}` and `${TM_CLICK_URL_URLENC}` in multiple places. The following example tag shows the inserted macros highlighted in yellow. 

<!--
![Example tag for Conversant](/help/dsp/assets/conversant_example_tag.png)
-->

<!-- Replace screen shot image with code block with appropriate highlighting once code highlighting is available. -->

<!--

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

-->

<!--
![flashtalking-logo1](/help/dsp/assets/flashtalking-logo1.jpg)
-->

Supported: iFrame & JavaScript tags

>[!NOTE]
>
>For each FlashTalking tag, you must manually insert the tracking macro `${TM_CLICK_URL_URLENC}` immediately before the URL in the `<a href>` tag and as the value of the `ftClick` variable. The following example tag shows the inserted macros highlighted in yellow.

<!--
![Example tag for FlashTalking](/help/dsp/assets/flashtalking_example_tag_snippet.png)
-->

<!-- Replace screen shot image with code block with appropriate highligting once code highlighting is available. -->
<!-- 

```
<noscript> 
<a href="${TM_CLICK_URL_URLENC}[http://servedby.flashtalking.com/click/8/57258;1799696;0;209;0/?ft_width=300&ft_height=250&url=9678632](https://servedby.flashtalking.com/click/8/57258;1799696;0;209;0/?ft_width=300&ft_height=250&url=9678632)" target="_blank"> 
<img border="0" src=" [https://servedby.flashtalking.com/imp/8/57258;1799696;205;gif;Tubemogul;300x250HTML5StandardwClickExtension/](https://servedby.flashtalking.com/imp/8/57258;1799696;205;gif;Tubemogul;300x250HTML5StandardwClickExtension/)?"></a> 
</noscript> 
<script language="Javascript1.1" type="text/javascript"> 
var ftClick = "${TM_CLICK_URL_URLENC}";
var ftExpTrack_1799696 = ""; 
var ftX = ""; 
var ftY = ""; 
var ftZ = ""; 
var ftOBA = 1; 
var ftContent = ""; 
var ftCustom = ""; 
var ftSection = " ${TM_SITE_ID_NUM}"; 
var ftID = function(){for(var e=["${USER_ID}"],a=e.length,r="";a--;)if(e[a]&&!RegExp("[^a-z0-9q-]".replace(/q/g,decodeURIComponent("%5"+"C")),"i").test(e[a])){r=e[a];break}return r}();; 
var ft300x250_OOBclickTrack = ""; 
var ftRandom = Math.random()&#42;1000000; 
var ftBuildTag1 = "<scr"; 
var ftBuildTag2 = "</"; 
var ftClick_1799696 = ftClick; 
if(typeof(ft_referrer)=="undefined"){var ft_referrer=(function(){var r="";if(window==top){r=window.location.href;}else{try{r=window.parent.location.href;}catch(e){}r=(r)?r:document.referrer;}while(encodeURIComponent(r).length>1000){r=r.substring(0,r.length-1);}return r;}());} 
var ftDomain = (window==top)?"":(function(){var d=document.referrer,h=(d)?d.match("(?::q/q/)+([qw-]+(q.[qw-]+)+)(q/)?".replace(/q/g,decodeURIComponent("%"+"5C")))[1]:"";return (h&&h!=location.host)?"&ft_ifb=1&ft_domain="+ encodeURIComponent(h):"";}()); 
var ftTag = ftBuildTag1 + 'ipt language="javascript1.1" type="text/javascript" '; 
ftTag += 'src=" [https://servedby.flashtalking.com/imp/8/57258;1799696;201;js;Tubemogul;300x250HTML5StandardwClickExtension/?ftx='+ftX+'&fty='+ftY+'&ftadz='+ftZ+'&ftscw='+ftContent+'&ft_custom='+ftCustom+'&ft_section='+ftSection+'&ft_id='+ftID+'&ftOBA='+ftOBA+ftDomain+'&ft_referrer='+encodeURIComponent(ft_referrer)+'&cachebuster='+ftRandom+](https://servedby.flashtalking.com/imp/8/57258;1799696;201;js;Tubemogul;300x250HTML5StandardwClickExtension/?ftx=%27+ftX+%27&fty=%27+ftY+%27&ftadz=%27+ftZ+%27&ftscw=%27+ftContent+%27&ft_custom=%27+ftCustom+%27&ft_section=%27+ftSection+%27&ft_id=%27+ftID+%27&ftOBA=%27+ftOBA+ftDomain+%27&ft_referrer=%27+encodeURIComponent(ft_referrer)+%27&cachebuster=%27+ftRandom+)'" id="ftscript_300x250" name="ftscript_300x250"'; 
ftTag += '>' + ftBuildTag2 + 'script>'; 
document.write(ftTag); 
</script>
```

-->
