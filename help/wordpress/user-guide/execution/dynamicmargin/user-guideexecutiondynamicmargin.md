---
edit-last: 4
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
pubDate: Thu, 14 May 2015 18:14:21 +0000
dc-creator: hthomas@adobe.com
guid: https://education.tubemogul.com/?page_id=3715
isPermaLink: false
description: 
postId: 3715
postDate: 2015-05-14 10:14:21
postDateGmt: 2015-05-14 18:14:21
commentStatus: open
pingStatus: open
postName: dynamicmargin
status: publish
postParent: 1424
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Dynamic Margin Management {#dynamic-margin-management}

Dynamic Margin Management is the second business model that is supported&nbsp;in TubeMogul's Margin Management feature. This option allows you to manage margins down to the placement level and optimize based on the financial efficiency of each placement. This feature&nbsp;gives you more flexibility than the Fixed Margin Management tool, but unlike that feature does not guarantee the margin %.&nbsp;It is up to the campaign manager to deliver the contracted units at or below their net margin to get the margin they want. This feature should be used if your client issues you an insertion order, consisting of several line items that you have agreed to deliver a fixed amount of units or unit types at a fixed rate. In the platform&nbsp;the insertion order is represented as a campaign,&nbsp;and line items are represented as [packages](../user-guide/execution/campaign-setup/packages/user-guideexecutioncampaign-setuppackages.md). Each package&nbsp;will have a specific goal, rate, and placements assigned to it. The placements can have different strategies and tactics organized to deliver the line item requirements, or in our case the "package goals" and "package rates". `<script src="//fast.wistia.com/assets/external/E-v1.js" async charset="ISO-8859-1"></script>` 
**Feature Setup:** `Step 1`: Navigate to the Campaigns page on the left hand side, and Create New Campaign. From there, fill out the Basic Campaign Details section. [ ![campaign basics](assets/campaign-basics1.png)](assets/campaign-basics1.png) `Step 2`:&nbsp;Fill out the Margin Management&nbsp;section of the page: [ ![image (7)](assets/image-7.png)](assets/image-7.png)

* Select "Yes" to activate Margin Management&nbsp;and "Dynamic"&nbsp;for the Margin Type
* Enter the Gross or Client's Budget
* Budget Reserve % is an optional safeguard, that can be used if you are not comfortable in putting the entire insertion amount as the spend cap. If during the campaign you are unable to deliver the contracted amount of units, you can make the decision on whether to increase your spend cap by reducing the reserve percentage.&#42;
* Spend Cap will be auto-calculated based on the Gross Budget and Budget Reserve %.

`Step 3`: Under Packages click Create a New Package. A new form&nbsp;will populate prompting you to fill in&nbsp;the following information: [ ![packages - campaign](assets/packages-campaign.png)](assets/packages-campaign.png)

* `Name`: Choose a name for your package
* `Dates`: Flight dates, note that all placements tied to this package must fall within these dates. These dates must also fall within the campaign flight dates.
* `Description`: Optional, if you'd like an additional description
* `Goal Type`: Select the metric&nbsp;that is your primary goal
* `Delivery Goal`: The number you'd like to deliver
* `Package Type`&#42;: The pricing method you'd like to track against
* `Package Rate`&#42;: The rate you'd like to track against
* `Budget` is then auto-calculated based on the above information, and used for tracking ONLY.
* `3rd Party Billed Fees`: Enter a consolidated CPM amount and 3rd party fee description. To see a walkthrough of this feature, [click here](http://fast.wistia.net/embed/iframe/rhi560hsx0?popover=true).

    * This feature does not override fees for services provided by TubeMogul such as Nielsen, comScore and IAS. &nbsp;To bring your own rate for these services, reach out to your Account Manager. These fees will be tracked as "non-billable other cost".

*&#42;Note, when using Packages to track dynamic margin these are the fields that are used to calculate that metric. Enter the type and rate that was sold to your client and the platform will track against these metrics. Once again, the platform will only track these metrics NOT cap delivery. Only margin at the campaign level (using fixed margin) will cap your spend.* **Feature Setup (Placement Level):** `Step 1`: Create a package when creating/editing a placement. [ ![package-placement](assets/package-placement.png)](assets/package-placement.png) `Step 2`: Either choose a Package that has already been created, or Create a New Package. If you are creating a new package, the same package form as above will populate. [ ![package-placement2](assets/package-placement2.png)](assets/package-placement2.png) This feature also allows you to set up 3rd Party Billed Fees at the placement level. [ ![3rdparty](assets/3rdparty.png)](assets/3rdparty.png)   &#42; *Note only include these fees if you have not done so at the package level, or if these fees should only be associated to a single placement within the package.* **Reporting:** This is accessible in different parts of the platform, depending on the feature. Margin Management can be found at the campaign and placement reporting pages, as well as exported at the bottom of each page. Revenue will encompass media cost as well as the margin you've obtained. [ ![reporting-mm](assets/reporting-mm.png)](assets/reporting-mm.png)   Package level reporting is accessible in 2 ways: `Option 1`: Filter placements by package association in the placement list page. [ ![package reporting1](assets/package-reporting1.png)](assets/package-reporting1.png)     `Option 2`: Export package level data by hitting "Export" button. [ ![pacakagereporting2](assets/pacakagereporting2.png)](assets/pacakagereporting2.png) &nbsp; In the exported page, analyze the data using the metrics below:

* Package name
* Margin % (if fixed margin or package rates are used)
* Profit
* Revenue (if fixed margin or package rates are used)
* Breakout of costs by TubeMogul billed (billable) vs 3rd Party Billed (non-billable)

    * Billable Media Cost
    * Billable Data Cost
    * Billable Other Cost
    * Non-Billable Media Cost
    * Non-Billable Data Cost
    * Non-Billable Other Cost - 3rd party billed fees will roll up here

&nbsp; If you have any additional questions, please reach out to your Account Manager or platform_support@tubemogul.com.&nbsp;To check out our Fixed&nbsp;Margin Management help page, [click here](../user-guide/execution/fixedmargin/user-guideexecutionfixedmargin.md). 