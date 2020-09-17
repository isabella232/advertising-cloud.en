# Best Practices for Setting up Performance Campaigns {#optimization-best-practices-performance}

Advertising Cloud can optimize your performance-focused campaigns for placements with the lowest cost per acquisition (CPA) or the highest return on ad spend (ROAS).

See the following best practices for performance campaigns:

* Step 1 - Define your Goal
* Step 2 - Define your Strategy
* Step 3 - Create Packages
* Step 4 - Create Placement Structure
* Step 5 - Use the Right Creative Assets

## Step 1 - Define Your Goal

It's important to understand whether the goal of the campaign is to achieve the highest possible ROAS or the lowest possible CPA. For each package in the campaign, you'll specify the objective goal accordingly as either *Highest ROAS - Custom Goal* or *Lowest CPA - Custom Goal*.

![optimization goal](/help/dsp/assets/optimization-goals.png)

You also need to determine the success event(s) that will lead to the overall goal and create custom goals accordingly. For each package, you'll specify a custom goal to be used with the overall optimization goal for reporting and algorithmic optimization using Adobe Sensei. For more information about creating custom goals, see the [Best Practices for Building a Custom Goal](custom-goal-best-practices.md).

![custom goals](/help/dsp/assets/objective-goals.png)

## Step 2 - Define Your Strategy

### Prospecting Strategies

Upper funnel packages include placements with very broad targeting to reach net new consumers.

#### Recommended Placement Strategies for Prospecting

* Find new audiences that are likely to convert using the following tactics:

  * Look-alike modeling from a data management platform (DMP), such as Adobe Audience Manager.
  * Behavioral targeting using third-party data.
  * Contextual targeting.
  * Site/category targeting.

* Use run of network (RON) targeting: It’s important to include a run of network placement without audience targeting and with broad inventory targeting. This allows the Adobe Sensei algorithm to find valuable users who may have newer cookies that haven't yet been categorized into an audience.

### Retargeting Strategies

Lower funnel packages include placements that target users who have already been to the advertiser's webpage or for whom the advertiser has CRM data.

#### Recommended Placement Strategies for Retargeting

* If the advertiser is an Adobe Analytics or Adobe Audience Manager customer, then you can build first-party segments (such as homepage visitors, product pages, or cart abandoners) and use them as placement targets in Advertising Cloud.

* Avoid assigning too much budget to an audience-targeted placement. As a general rule, budget $30 per 1,000 users per month.

## Step 3 - Create Packages

The best practice is to create separate packages for upper funnel prospecting and for lower funnel retargeting. Optimization occurs at the package level, so that performance data from all placements within a package is pooled. Therefore, group placements into packages with similar expected performance.

![example of separate packages for prospecting and retargeting](/help/dsp/assets/p-r.png)

Also, use the following settings.

### Goals & Budget

* **Pacing & Capping:** To select a CPA or ROAS optimization goal, the package must use package-level pacing. This ensures that all placements within the package are optimized to distribute spend based on performance and scale to the selected goals.

* **Flight Dates:** (Prospecting packages) When your campaign runs for longer than 25 days, use the Activate Custom Flighting feature. First, set a custom flight for the first 10 days at approximately 75% of the necessary daily budget to reduce spending during the *learning phase*. Then set a second custom flight for the remainder of the budget.

  For example, if you have $100,000 to spend in 30 days, then set the budget for Flight 1 (Days 1-10) to $25,000 (75% x $100,000/30 days = $2,500 per day). Use the remaining budget of $75,000 for Flight 2 (Days 11–30).
  
* **Budget:** DSP will always try to allocate 100% of the package budget evenly between all placements in a package. If a placement has low spend or no spend, we recommend budget capping the placement to allow more of the budget to allocate to placements with scale. Allow 24-48 hours for budget changes to calibrate.

* **Optimization Goals:** Use one of the two performance optimization goals, *Highest ROAS* or *Lowest CPA*, depending on the package goal. These goals auto-optimize the package towards the Highest ROAS or Lowest CPA placements, respectively.

* **Custom Goals:**
  * If a new package has the same goal as an existing package, you can optionally link the existing package so that the algorithm can use the existing machine learning data.
  * Enter the appropriate Target CPA or ROAS.

* **Pacing Fill Strategy:** Select *Even* to maximize your performance goals by pacing uniformly throughout the entire flight date.

  Use *FrontLoad* and *Aggressive Front Load* pacing only when you are fully prioritizing delivery and spend over performance optimization because those strategies can negatively impact your desired performance KPIs.

## Step 4 - Create Placement Structure

Less is more. If you can set up fewer than six placements per package, then the available budget can dynamically shift to the best performing placements most easily.

Also, make sure to add each placement to a package with a package goal type of *Prospecting* or *Retargeting*, as appropriate.

The following are the recommended placement settings for performance campaigns.

### Goals

You'll configure CPA or ROAS optimization at the package level (see Step 3 - Create Packages), but you can add additional placement-level settings.

* **Max Bid:**
  * For prospecting placements, use a low maximum bid ($5).
  * For retargeting placements, use a high maximum bid ($12).

* **Pre-bid Filters:** Minimize, or ideally avoid, setting aggressive pre-bid filters, which prevent the placement from achieving scale. Best practices include the following:

  * Use one (1) pre-bid filter per placement. Multiple pre-bid filters will require that both are met, which reduces scale.

  * Consider setting less strict pre-bid filters in cases where additional targeting (such as audience, geo, and site targeting) is applied.

See descriptions of when to use each pre-bid filter at [Placement-level Pre-Bid Filters and How to Use Them](/help/dsp/optimization/optimization-pre-bid-filters.md).

### Inventory

To maximize scale, use Public (Open Exchange) and On Demand inventory.

### Site Targeting

* **Traffic Type**: Websites only
* **Site Tier**: All sites

### Audience Targeting

* **Included Audiences:**
  * For prospecting placements, group similar audience categories and similar audience sizes into one placement. Then, based on performance, do one of the following:
    * Remove under-performing audiences from existing placements.
    * Move top-performing audiences into a separate placement to better control budgets.
  * For retargeting placements, you should ideally include one audience segment per placement to easily control bids and budget.
  
>[!NOTE]
>
>Your ads will perform best if a user can be reached by only one placement. Significant overlap in users across placements can cause competition, which yields a cycle of continually increasing bids, driving up the cost per user. Therefore, if you include multiple audiences, make sure they don't consist of overlapping users/audience members.
>
> You can avoid overlapping audiences by creating your audiences in tiers so that you can suppress the higher, more inclusive tiers from placements as needed.

* **Frequency Capping:**
  * For prospecting placements, use tight frequency caps (one impression per day).
  * For retargeting placements, set the primary placement cap to 6-10 impressions per day, and the secondary cap to one impression per hour.

* **Device Targeting**:
  * Include Computer, Mobile, and Tablet.
  * Don't target Firefox, Safari, or IE 6, 7, or 8 because of targeting and measurement limitations. Contact your Adobe account manager for more details about Adobe support for Safari ITP.
  * If you target mobile web traffic, then disable all mobile browsers except Chrome and Edge.

### Brand Safety and Media Quality

Using contextual filtering, pre-bid fraud blocking, and/or Ads.txt filtering will limit the scale of your placements, but use them if needed.

## Step 5 - Use the Right Creative Assets

* The best practice is to include as many unique ad sizes as possible to maximize reach. The universal display template allows you to upload any standard display ad size.
* Make sure all placements contain *at least* all of the primary display ad sizes (300x250, 728x90, 160x600, 300x600, 320x50, and 300x50).
* Update creatives frequently to prevent creative fatigue.

>[!MORELIKETHIS]
>
>* [Package Settings](/help/dsp/campaign-management/packages/package-settings.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
> * [How DSP Optimizes Your Campaigns](optimization-how-dsp-optimizes-campaigns.md)
>* [Optimization Goals and How to Use Them](optimization-goals.md)
>* [Placement-level Pre-Bid Filters and How to Use Them](optimization-pre-bid-filters.md)
>* [Campaign Launch Checklist](/help/dsp/campaign-management/campaign-launch-checklist.md)