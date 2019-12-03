---
edit-last: 4
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
pubDate: Fri, 04 Jul 2014 15:48:37 +0000
dc-creator: hchang@adobe.com
guid: https://education.tubemogul.com/userguide/?page_id=1416
isPermaLink: false
description: 
postId: 1416
postDate: 2014-07-04 07:48:37
postDateGmt: 2014-07-04 15:48:37
commentStatus: open
pingStatus: open
postName: brandpoint
status: publish
postParent: 1408
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# BrandPoint {#brandpoint}

BrandPoint is the simplest and most cost effective way to buy video advertising using Gross Rating Points (GRPs). BrandPoint enables brand marketers to plan, buy and measure digital video on a comparable basis to TV. For the first time, advertisers can execute verifiable and optimized delivery to online populations – dynamically. BrandPoint buys media in real-time, to reach a client’s desired audience. [Nielsen](../../dsp/measurement/nielsen-ocr-reporting.md) and [Comscore](../../dsp/measurement/comscore-vce.md) validated reporting are also available within the dashboard to measure and verify delivery.

Media buyers are looking to supplement their TV buys with online video, but they need a reliable and simple platform for buying and executing a GRP buy. BrandPoint will not only accurately predict a buy, but also uses proprietary data targeting to provide the best Cost Per Point in the industry.

## How BrandPoint Works

[ ![how it works](assets/how-it-works.jpeg)](assets/how-it-works.jpeg)

## How Cost Per Point Is Calculated

Advertising Cloud DSP uses proprietary data targeting to improve on-target % throughout the campaign. BrandPoint calculates the Cost Per Point using several different factors:

* Sites: Advertising Cloud DSP indexes inventory using Nielsen OCR and Facebook-based user data. These two methods provide BrandPoint site-level demographic breakdowns for our inventory.
* Audience Data: Advertising Cloud DSP machine learning creates large pools of users and maps them to age and gender combinations. These pools of users are created using look-alike modeling based on validated truth sets. We test this data using Nielsen OCR and create a database of on-target percentages for each pool of users. The data is then applied to campaigns bought on a CPP.
* Inventory Cost: BrandPoint has historical auction data of expected cost of inventory from billions of auctions that Advertising Cloud DSP sees on a daily basis.

Our tool combines the above data points to calculate the Cost Per Point of a campaign. The process takes the following steps:

1. BrandPoint determines how many impression you'll be able to buy given your budget and targeting parameters
1. BrandPoint calculates how many of those impressions will be on target. This blends both the site demographics data and the audience segment data together.
1. BrandPoint calculates how many GRP's your plan will achieve using the digital GRP formula.

## How to Calculate a Digital GRP

Below is the formula BrandPoint uses to calculate GRP:

`GRP = (Total impression * On-Target%)/Natural Population`

where Natural Population is your total target population. For example, if you are targeting Female 25-54 in the US, the population number you would use is 62.8M. If you were targeting a specific DMA, the population number would be based on that DMA. To maintain consistency with Nielsen TV GRP calculations, "Natural Population" is using overall population rather than online audiences only.

## Supported Ad Formats

BrandPoint is available for the following ad formats:

* Pre-roll
* Interactive Pre-roll
* Skippable Pre-roll
* Click-to-Play
* Rollover-to-Play
* Branded Autoplay
* Fullscreen Expandable
* Facebook CPV

## Available Countries

* Americas: United States, Canada
* Europe: United Kingdom, France, Spain, Germany, Italy, Ireland, Sweden, Norway, Finland, Romania, Denmark, Netherlands, Switzerland, Belgium
* APAC: Australia, Japan, Indonesia, Taiwan, Thailand, Malaysia, Hong Kong, Singapore, Philippines, Vietnam, China, South Korea

## Audience Reporting

In-product Nielsen OCR reporting is available in the US, UK, Australia, Germany, Italy, Brazil, and France. For all other countries, Advertising Cloud DSP offers its own demographic reporting.