---
edit-last: 43
wp-page-template: default
rawhtml-settings: 0,0,0,0
ldc-disable: 0
ldc-disable-comm: 0
pubDate: Fri, 12 Jul 2019 14:26:29 +0000
dc-creator: siddbhat@adobe.com
guid: https://education.tubemogul.com/?page_id=7715
isPermaLink: false
description: 
postId: 7715
postDate: 2019-07-12 06:26:29
postDateGmt: 2019-07-12 14:26:29
commentStatus: open
pingStatus: open
postName: performance-display-playbook
status: publish
postParent: 7518
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Performance Display Playbook {#performance-display-playbook}

1. Defining your goal
1. Defining your strategy
1. In-platform Set-Up
1. Placement structure
1. Creative


## Step 1 -  Defining your goal

It is important to understand the goal of the campaign, whether Cost per Acquisition (CPA) or Return on Ad Spend (ROAS), and the success event(s) that lead to the overall goal.

Ad Cloud has the ability to report and optimize towards a single or multiple success events through our Custom Goal tool. Once the Custom Goal is created, you can assign it to your campaign's package for reporting and algorithmic optimization.

![objective goals](assets/objective-goals.png)

Follow this link for the

[Building a Custom Goal Playbook](https://education.tubemogul.com/?p=7818)

## Step 2 - Defining your strategy

### Prospecting

(Upper Funnel) packages are comprised of placements with very broad targeting to reach net new consumers. Applying tactics such as Lookalike modeling, Behavioral Targeting (3rd party data), Contextual Targeting, and Site/Category Targeting findsnew audiences that are likely to convert. 
Recommended Strategies`: **DMP Lookalikes** (Adobe Audience Manager, etc.) and **RON** (Run Of Network) 

>[!NOTE]
>While lookalike modeling and 3rd party data are key tactics to identify new users, it’s important to also include a Run of Network placement without audience targeting and with broad inventory targeting. 
>
>This leverages the full power of the machine learning algorithm to find valuable users who may be newer cookies not yet categorized into an audience.

Recommended Settings:

* Low max bid ($5)

  ![max bid 5](assets/max-bid-5.png)

* `Tighter frequency caps(1x per 24 hours)

  ![](assets/freqap-playbook.png)

* `Package Custom Flighting: Ifyourcampaignextends past25 days, setacustom flight forthefirst 10 days at ~75% ofthenecessary daily budget to reduce spending duringthe ‘learningphase’.Seta2nd custom flight fortheremainder ofthebudget to spend in full.

  ![](assets/custom-flighting.png)

* Example: 
  ```if you have $100K *to spend in* * `30 days, set Flight 1`* * `’s`* * `budget (days 1-10) to $25,000 (75`* * `%`* * `*`* * `$`* * `100,000/30`* * `days`* * `=`* * `$`* * `2,500 per day). Flight 2 (days 11 – 30) will be the remaining budget of $75,000.`*```

### Retargeting

(Lower Funnel) packages are comprised of placements targetingusers who have already been to the advertiser's webpage(s) or CRM data.

*Recommended Strategies*: If the advertiser is an Adobe Analytics and/or Audience Manager customer, you can build and pass first party segments to Ad Cloud for targeting.(homepage visitors, product pages, cart abandoners, etc.) 

![Marketing cloud segments](assets/marketing-cloud-segments.png)

Avoid assigning too much budget to an audience-targeted placement. As a rule of thumb, we should budget $30 for every 1,000 usersper month.

Recommended Settings: 

* Higher max bid ($12+)

  ![max bid 12](assets/max-bid-12.png)

* Frequency Caps for Retargeting: Primary Cap of 6 impressions per day, Secondary Cap of 1 impression per 1 hour on the Package Level ``

  ![](assets/rt-freq-caps.png)

Suppression is key to driving efficiency. When using multiple retargeting audiences, it’s important totierthem and suppress higher tiers from each placement underneath. 

Ultimately you will drive the best performance if a user can only be reached by one placement. If there is significant overlap in users between placements, it can causecompetition which yields a cycle of continually increasing bids, driving up the cost of a user.

## Step 3 - In-Platform Set-Up

### Package structure

Best practice is to have separate packages for upper funnel prospecting and lower funnel retargeting. Ad Cloud’s optimization occurs at the package level, so performance data from all placements within a package is pooledtogether. Placements should be grouped into packages with similar expected performance.

![P & R](assets/p-r.png)

1. **Basic Details**: (fill inPackage Name,Description, etc.)
1. **Goals and Budget**: Packages must be set to `Package level pacing` to activate CPA or ROAS optimization. Enabling this feature will auto-optimize towards the Lowest CPA or Highest ROAS placements.   

1. **Activate Custom Flighting**: if your flight extends past 25 days

   ![Create a Package](assets/create-a-package.png)

1. **Optimization Goals**: There are two performance Optimization Goals – **Highest ROAS** and **Lowest CPA**.  You will need to select one of these Optimization Goals depending onyourgoals. 

   ![Opt Goakl](assets/opt-goakl.png)

1. **Custom Goals**: Choose your campaign(s) Custom Goal
   * If you have packages using the same Custom Goal, you have the option to link a new package to an existing package for machine learning / algorithm carryover. 
   * Add Target CPA or ROAS

1. **Set package Pacing Fill Strategy**: to *Even* to maximize your performance goals. 

   Applying *FrontLoad* and *Aggressive Front Load* pacing is only recommended when you are fully prioritizing delivery & spend, as these two pacing strategies can negatively impact your desired performance KPIs (as it will prioritize delivery over performance optimization).

   ![Pace On](assets/pace-on.png)

   * Even: Pacing will be uniform throughout the entire flight date
   * FrontLoad: Pacing is accelerated at the beginning to be 15% ahead of pace by mid-flight
   * Aggressive Front Load: Pacing is accelerated at the beginning to be 25% ahead of pace by mid-flight. The algorithms won't be very effective when using this pacing strategy

## Step 4 - Placement structure

Less is more! If you can set up less than 6 placements per package, this maximizes the available budget to dynamically shift to the best performing placements.

1. **Goals** CPA or ROAS optimization is done at the package level, but there are placement level settings that can be added. Minimize (ideally avoid) use as setting overly aggressive prebidfilters will have a negative impact on the placements ability to scale

1. **Inventory** Public (Open Exchange) and On Demand are recommended to maximize scale

   ![Screen Shot 2019-07-12 at 7.39.19 AM](assets/screen-shot-2019-07-12-at-7.39.19-am.png)

1. **Site Targeting**

   * **Traffic Type**: Websites only 
     >[!NOTE]
     >Adobe Ad Cloud conversion pixels currently do not track mobile app delivery

   * **Site Tier**: Allsites

     ![Site vs app](assets/site-vs-app.png)

1. **Audience Targeting**:

* Prospecting: Suggest grouping similar category and sized audiences into one placement. Based on performance, do one of the following:
  * Remove under-performing audiences from existing placement
  * Breakout top performing audiences into a separate placement to better control budgets
* Retargeting: Suggest one audience segment per placement to easily control bids and budgets

  >[!NOTE]
  > If running multiple audiences, it is recommended to suppress the audiences from each other to avoid overlap

  * Prospecting Audience(s): $5 Max Bid
  * Retargeting Audience(s): $12 Max Bid

5. **Frequency**:
   * **Prospecting**: 1x per day
   * **Retargeting**: 3x – 6x per day 

1. **Device Type**: Include Computer, Mobile, and Tablet

   * Do not target IE 6, 7, or 8 and Safari due to targeting and measurement limitations (reach out to your Account Manager for more details on Adobe & Safari ITP)
   * If targeting mobile web traffic,disable all mobile browsers besides Chrome, Firefox, and Edge

   ![device targeting](assets/device-targeting.png)

1. **Brand Safety and Media Quality** Enabling Contextual filtering, Pre-bid fraud blocking, and/or Ads.txt filtering will limit your placements’scale butcan be set if needed.

## Step 5 - Creative

* Best practice is to include as many unique ad sizes as possible to maximize reach.  Adobe's universal display template allows you to upload any standard display ad size
* Make sure all placements contain *at least* all of the primary display ad sizes (300x250, 728x90, 160x600, 300x600, 320x50, and 300x50)
* Update creative on aregular basis to prevent creative fatigue

