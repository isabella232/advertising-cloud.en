---
edit-last: 43
wp-page-template: default
rawhtml-settings: 0,0,0,0
ldc-disable: 0
ldc-disable-comm: 0
pubDate: Mon, 04 Mar 2019 22:49:40 +0000
dc-creator: siddbhat@adobe.com
guid: https://education.tubemogul.com/?page_id=7623
isPermaLink: false
description: 
postId: 7623
postDate: 2019-03-04 14:49:40
postDateGmt: 2019-03-04 22:49:40
commentStatus: open
pingStatus: open
postName: audio-faq
status: publish
postParent: 7619
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Audio FAQ {#audio-faq}

## General {#customerfacingfaqs-general}

* What are the category restrictions for each pub?

  * Spotify -  [see here for full list](https://www.spotify.com/us/brands/legal/advertiser-terms-and-conditions/)

    * Blacklist - Adult products (tobacco, marijuana, illegal drugs, online prescription pharmacies, sexually explicit content, etc.), dangerous weapons, illegal products, cryptocurrencies, etc.

      * Political campaigns are blacklisted through always on deals but allowed on a case by case basis. Please work with your account manager for PMP set-up details.

      * Restricted (allowed with some limitations) - alcohol, online dating services, gambling, lotteries, contraceptives, supplements, competitive products to Spotify, financial, insurance, religion, etc.

    * Soundcloud -  [see here for full list](https://advertising.soundcloud.com/policies)

      * Blacklist - products/services that infringe 3rd party rights, illegal drugs, adult products, tobacco, other financial (see below for approved financial), dangerous weapons, political (non-profit awareness or charity groups are ok), religion, etc.
      * Restricted (allowed with some limitations) - financial (retail banks, mortgage lenders, insurance companies), alcohol, marijuana, non-prescription pharma, contraceptives, medical products, online dating services, gambling, lotteries, etc.

    * TargetSpot, TuneIn and iHeart

      * Restricted - marijuana (creative review required).

* The client doesn't have audio assets - is there a creative service that offers script creation & narrative/voice-overs?

  * Spotify can create an audio asset for clients with a guaranteed spend commitment. Please reach out to your account manager for details.
  * TuneIn has audio studios in LA and SF; no minimums but ask that you spend audio budgets with them
  * iHeart studio can produce basic audio assets. They offer this service as added value with a large budget commitment or with a guaranteed spend amount. Please reach out to your account manager for details.
  * TargetSpot has a partner that can produce audio assets.They offer this service with a guaranteed spend commitment. Please reach out to your account manager for details.
  * We recommend that customers use  [VoiceBunny](https://voicebunny.com/#/) (low production costs and 24hr turn around time).

* How do audio publishers gather geo data?

  * Usually IP from users' devices

* Do our audio partners offer call centers? (i.e., Dial #250 and say the keyword PIZZA to get your free Dominoes coupon texted to you.." in an audio ad)

  * Only iHeart has this option

* Why is my advertiser getting blocked from Audio publishers in the On Demand Gallery?

  * Make sure the Advertiser Category (found within the edit Campaigns section of the UI) is accurate and not 'Other' - as 'Other' will automatically be blocked. Certain categories are restricted from running on Audio publishers, please see the first question on this FAQ doc re: category restrictions

* Is audio a brand safe environment?

  * Pre-bid and contextual features are not available on audio placements. But, we do not support any pre-bid filtering for any mobile app inventory, so audio is in line with that.

    * That being said, some brand safety categorization is primarily on non-audio components (i.e., url, test, content)
    * `Oracle (Moat/Grapeshot):` page-level categorization is based on text / other content on the page. Audio files are not mapped in most cases, unless available to Oracle. They are currently working with Spotify to enable audio categorization of their inventory.
    * `DoubleVerify:` Based on page/domain/device identifiers, rather than the audio asset
    * Adswizz is unable to send URL domains in some cases because it is controlled by the publishers. If publishers don't fill in the domain, Adswizz cannot pass that through.
    * iHeart, TuneIn, etc has thousands of domains due to the sheer amount of radio stations, they do not always fill in the domain names
    * When we have no domains to work with, it means we cannot use contextual services for brand safety - it would cause no bids.
    * Proximic topic targeting is enabled on audio placements - be aware this can impact your audio bids if you are running on Adswizz or other partners that do not pass through domains

    * Audio is generally a brand safe environment since all content is curated by publishers/partners and in closed environments.

* Do I still need to "whitelist" my advertiser for Audio?

  * No, no more need to whitelist your advertiser for audio. All you will need to do is target whichever feed you'd like - just make sure your advertiser "category" is accurate! Certain categories are restricted from running on audio feeds, such as political.

### Podcasts {#customerfacingfaqs-podcasts}

* Can we run on OnDemand for TargetSpot's podcast inventory?

    * Yes

* Can we cherry pick podcasts to run on? How can we ensure a brand safe environment?

    * TargetSpot will allow you to choose  `categories` of podcasts through direct deals, but not specific podcasts
    * SoundCloud is only run of podcasts
    * Brand Safety: All podcast content is verified by the audio partner
    * For full podcast lists, please go to  [TargetSpot](https://wiki.corp.adobe.com/display/TMCS/TargetSpot) or  [SoundCloud Partner Materials](https://wiki.corp.adobe.com/display/TMCS/SoundCloud)

<!-- Two links above are to wiki.corp.adobe.com. Users outside the Adobe firewall won't be able to view those links. Make public? Remove? Add "(Internal Only)"? -->

* Do ads on podcasts run on pre- mid- or post- roll?

    * Podcast ads will run pre-roll on SoundCloud and mix of all three types on TargetSpot

* How can we avoid being co-promoted with competitors within podcasts?

    * Targetspot: No way to avoid this right now due to technical reasons. It is something they are looking to improve upon in the coming months.
    * SoundCloud: All inventory, including podcasts, is pre-roll. No risk of co-promotion during a podcast since only one ad plays before each podcast starts. SoundCloud podcasts are not host-controlled advertising, meaning there is no host giving a quick vocal promo.

## Connected Devices {#customerfacingfaqs-connecteddevices}

* What connected devices can we run ads on for audio?

  * Sonos and Echo (through TuneIn inventory, which is an app that comes pre-installed on these devices)
  * No other audio partners currently offer connected device targeting
    >[!NOTE] 
    >Spotify Free is not available to stream via Amazon Alexa devices

## Measurement {#customerfacingfaqs-measurement}

* Can we gather device IDs from audio?

  * Yes, only on mobile devices

* Can we ingest Audio metrics back into Analytics (AA) workspaces via Reverse Feed for conversions and attributions?

  * Yes, we can confirm that AA conversions are being matched against audio ads. Please note that it will only work for same-device, cookie environments ONLY.

* Can we run Adobe Surveys off exposed audio impressions?

  * Yes, we can run Surveys on mobile devices with audio exposure (as we receive device IDs from mobile audio impressions)

* Can we run any third party studies across audio?

  * Yes, we can run a Placed Study

* Are we able to measure conversions on audio?

  * Yes, only for desktop web right now. Audio is a part of our attribution service. If you take a look at the Attribution sharepoint page it outlines our measurement capabilities and that we can track audio as part of MTA for desktop web.

* Can we run Nielsen for OTP measurement?

  * Yes, but it varies by publisher and platform. We are currently testing pixel certification as our platform only generates web-only Nielsen pixels - stay tuned for cross-device pixels & results!

* Can we report on audience overlap or unique reach/frequency?

  * No, Facebook has shuttered the AMT tool we used to report on audience overlap. This is not longer available. Reach out to the AMS team for a new solution.

* Can we control frequency on feeds?

  * Yes, you can frequency cap using the device ID for all audio partners.
    * Caveats:

      * Spotify currently defaults to 3 ads per 24hr frequency cap applied to all deals; if you set a more strict cap at the placement level it will be respected
      * Some private deals through Adswizz may not be able to because the user macros were not added to the VAST tag on Adswizz's end (you have to ask them to do that)

* Which 3rd party pixels can I append to audio ads?

  * Most 3rd party pixels will work on audio ads for impression/click tracking - make sure you are using IMG URL pixels, not HTML

* What are the metrics for podcast inventory?

  * Impressions and completions are the main metrics you will see on a TargetSpot podcast buy. As long as the user listens to the podcast within 3-5 business days we will serve the ad and the imps/completion pixels are fired. Anything past that time frame our pixels time out and the user will not receive an ad before their podcast.

### Targeting {#customerfacingfaqs-targeting}

* Can we target 3rd party data on audio?

  * Yes, any of our audio providers that can pass back IDs/cookies can be matched in our system when targeting data and bought on - If there’s scale.
  * Spotify would need mobile data (device IDs). Spotify desktop is in-app, so no cookies.

* Can we target 1st party CRM data on audio?

  * Yes, in general you can target AA and AAM data (if the client has these solutions). Again, scale would need to be monitored, and data would need to match the targeted devices (cookies for desktop, device IDs for mobile).
  * For Spotify, 1st party CRM data can only be used on mobile - advertisers must send Spotify their customer data in advance of the campaign going live either thru Google's Guaranteed Audience product (upload into DV360 to push over) or Custom Audience Match via our integrations with Liveramp and Adobe. Both are in beta so there is some testing involved.

    * For PMPs, they must confirm their audience pool has device IDs to match with our mobile inventory only (no desktop because no identifier). They then need to confirm how big that pool is so we know whether there is scale.

* Can we use Spotify's 1st party data (genre, playlist, etc.)?

  * Yes but only in desktop environments (due to GDPR, needing to protect our data that can be leaked if being applied to mobile inventory because mobile passes a device ID back in the bid request that gives partners knowledge on the user that is private to Spotify)

* Can we retarget audio audiences on other channels?

  * Yes, since all our audio providers pass back device IDs/cookies, we can target across channels. However, it is only parallel retargeting right now - mobile to mobile, desktop web to desktop web (i.e., Spotify mobile → mobile pre-roll ; iHeart desktop → desktop display)

* Can we Behavioral Target on our audio partners?

  * Yes, the only restriction is not on Spotify desktop because it is a cookieless enviroment.

* Can we target audiences who have paid and/or free audio subscriptions?

  * Only targeting free subscription audiences.

* How do audio partners know age, demo, or location of their audiences?

  * Partners gather this information upon users' registration.

* Can we target by zip/geo/postal code?

  * Yes, this isn’t limited by publisher, we have the ability to geotarget the same way as we do with mobile video or display. You may experience scale issues depending on any other targeting, limitations, etc.

* Can you negatively target/blacklist within Audio? If so, is that by genre?

  * No, whitelisting only within our UI. The publisher can negatively target for the client if they set up a private deal

### Ads {#customerfacingfaqs-ads}

* Do we have to add companion banners?

  * No, companion banners are optional, but strongly recommended! If you do not submit a companion banner, the audio partner will often auto append a branded one for you (i.e., Spotify Ads, SoundCloud Ads).

* Where will I see companion banner clicks in the UI?

  * Companion banner clicks will appear in the "Companion Clicks" field in the placement list page. "Total Ad Clicks" does not include companion banner clicks.

    * Exception: For Spotify only, all companion banner clicks will show up under "Banner Clicks".

* Can you upload more than one companion banner to an ad, and have it auto rotate?

  * No, please create multiple ads with unique companion banners and have them rotate that way.

* Do I have to submit a click URL?

  * No, click URLs are not mandatory, and will make the companion banner un-clickable.
  * If you submit a click URL but not a companion banner, the branded companion banner (i.e., Spotify Ads, SoundCloud Ads) will click through to your specified destination

* Can we run completely without a companion banner?

  * No, as audio partners will append their own.
  * Note that not all audio ads will have companion banners (likely less than pre-roll shows companion banners), due to the nature of the ad (usually in the background, while phone is on lock).

* Can ads be longer than 30 seconds?

  * Yes, depending if partners will accept them on their end. Please reach out to your account manager for details

### Benchmarks {#customerfacingfaqs-benchmarks}

* VCR - 97% (On Demand)
* CTR - 0%-0.1%

  * All audio publishers (except TargetSpot) support companion banners. However, audio ads are served when the user Is not visually engaged with the device. Hence why click counts are low on audio campaigns.

* Viewability - n/a

  * Not a standard metric for audio ads, as they are normally served when the user is not visually engaged with the device
