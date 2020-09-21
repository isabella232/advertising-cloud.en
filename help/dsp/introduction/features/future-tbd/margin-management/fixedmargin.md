---
title: Fixed Margin Management
description: Fixed Margin Management
---

# Fixed Margin Management

Fixed Margin Management is one of the two business models supported in the Margin Management feature. In the past, you were asked to calculate the net budget outside of the platform, and then apply these at the campaign and placement levels. Now you can enter a gross budget, enter the pre-negotiated fixed margin percentage, and then Advertising Cloud DSP will auto-calculate and cap spend at the net budget.

Activating this feature at the campaign level will account for it at all levels. Ultimately reducing the amount of manual work required to figure out what your budgets are.

<!--
[ ![fixed](/help/dsp/assets/fixed.png)](/help/dsp/assets/fixed.png)
-->

## Feature Setup

Step 1: Navigate to the Campaigns page on the left hand side, and Create New Campaign. From there, fill out the Basic Campaign Details section.

<!--
[ ![campaign basics](/help/dsp/assets/campaign-basics1-1024x428.png)](/help/dsp/assets/campaign-basics1.png)
-->

 Step 2:  Fill out the Margin Management section of the page:

* Select "Yes" to activate Margin Management and "Fixed" for the Margin Type (cannot be changed once the campaign is created).
* Enter the Gross (Client's) Budget and Fixed Margin % - Using the example above of $10,000 and 10%, the platform will auto-calculate the Spend Cap (or net budget) of $90,000.

<!--
[ ![image (11)](/help/dsp/assets/image-111.png)](/help/dsp/assets/image-111.png)
-->

## Reporting

Reporting accessible in different parts of the platform, depending on the feature.

Margin Management can be found at the campaign and placement reporting pages, as well as exported at the bottom of each page. Revenue will encompass media cost as well as the margin you'd entered at either the campaign or package level.

<!--
[ ![reporting-mm](/help/dsp/assets/reporting-mm.png)](/help/dsp/assets/reporting-mm.png)
-->

Package-level reporting is accessible in 2 ways:
* Option 1: Filter placements by package association in the placement list page.

<!--
[ ![package reporting1](/help/dsp/assets/package-reporting1.png)](/help/dsp/assets/package-reporting1.png)
-->

* Option 2: Export package level data by hitting "Export" button.

<!--
[ ![pacakagereporting2](/help/dsp/assets/pacakagereporting2.png)](/help/dsp/assets/pacakagereporting2.png)
-->

In the exported page, analyze the data using the metrics below:

* Package name
* Margin % (if fixed margin or package rates are used)
* Profit
* Revenue (if fixed margin or package rates are used)
* Breakout of costs by Advertising Cloud DSP-billed (billable) vs third-party-billed (non-billable)

    * Billable Media Cost
    * Billable Data Cost
    * Billable Other Cost
    * Non-Billable Media Cost
    * Non-Billable Data Cost
    * Non-Billable Other Cost - 3rd party billed fees will roll up here

>[!MORELIKETHIS]
>
>[Dynamic Margin Management](dynamicmargin.md)
