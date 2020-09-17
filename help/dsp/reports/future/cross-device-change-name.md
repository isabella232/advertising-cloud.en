

For Cross-Device Targeting & Frequency Management  

Creating a New Campaign with a device graph enabled:  

Under the “Campaign Goals” section, you will see a “Cross Device Level” field which by default will be at “Same Device”. To enable cross-device, switch this selection to “People”.  

You will then be prompted to select a Device Graph.  All Advertising Cloud DSP customers will have access to leverage the LiveRamp device graph. For Adobe Device Coop participants, connect with your Account Manager to provision your DSP account advertiser with access to this graph.  

Keep in mind that the Cross Device Level and Device Graph settings CANNOT be changed once the new campaign has been saved. However, you will be able to adjust frequency intervals (2 per day) and turn cross-device targeting on or off throughout your campaign.    

 

Creating a Package with a device graph enabled:  

Cross-device capabilities carry down from the Campaign selection so no changes are necessary during Package creation. That said, if you typically set up Frequency caps at the package level, we recommend modifying your cap interval to accommodate for this cross-device strategy.   

 

 

Creating a Placement and enabling Cross Device Targeting:   

When creating a placement under a Campaign that has been enabled with “people” level and a device graph, upon selecting audience segments to target, you will see a new “Cross Device Targeting” toggle. Turning this “On”, allows the system to take your original targeted segment and find these users across their other connected devices.   

A few details to keep in mind:  

Device Graph Vendor 

Data geo- restriction 

Cost for Cross Device Targeting * 

LiveRamp 

US  

$0.35 CPM for extended impressions only 

Adobe Device Coop 

US & Canada  

Free of charge 

* There is no cost for leveraging either graph vendor for frequency management or attribution measurement.  

 

Setting Up Reporting on Cross Device Extended Impressions:  

Once you’ve enabled Cross Device Targeting for certain audience targeted placements, we recommend setting up your custom email report to include our new cross device “Extended Impressions” metric. This metric allows you to understand the impact of leveraging a device graph for targeting and the number of impressions you otherwise would not have been able to serve to your customer if you had not leveraged a device graph.  

Device Graph (for Targeting) can be found in the Dimensions> Campaign section:  

This metrics allows you to track the device graph vendor used for a particular campaign, package or placement.  

 

 

Extended Impressions can be found in the Metrics> Standard Metrics section:  

This metric is the total number of impressions served as a result of leveraging a device graph for people based cross-device targeting.  This is also the metric used to calculate any applicable fees associated to using a 3rd party device graph vendor such as LiveRamp.  These fees will be rolled up into the Spend Metric “Other Net Spend”.  

 

Example of a report: Columns in green are specific to this offering.  

 

Common questions:  

Where can I see the cost of leveraging the graph?   

You can see this via your Account Rate Card 

If you want to aggregate costs across your campaign, the cost of leveraging the device graph for cross-device targeting will be aggregated under “Billable Other Net Spend”.  Keep in mind this metric includes all other fees you may apply to your campaign.  

Where do I find the  

 

Enabling Person-Based Attribution Measurement  

If you already implemented the Advertising Cloud Conversion pixels on your site and would like to activate “Cross-device attribution” measurement, connect with your Account Manager to enable.   

How to check when a device graph has been enabled for attribution measurement for your advertiser  

On the left navigation bar, go to Settings> Advertiser  

Find the Advertiser in question and click “Edit”  

Scroll down to Integrations > Cross-device attribution  

Example of an activated advertiser:  

 

Setting up automated custom reporting with cross-device conversions 

Once a device graph has been enabled for attribution measurement, you will notice the following new metric you can choose from within the "Conversion Report” template:  

Conversions (tp):  Total conversions including both same device and cross device (if applicable). 

Conversions (sd): Conversions where only one device was present in the conversion path. In the report, next to your conversion metric name and rule type, you will see (sd). 

Conversions (xd): Conversions where more than one device was present in the conversion path. In the report, next to your conversion metric name and rule type, you will see (xd). 

 

 

 

Example of columns that may show up in your conversion report: 

Sign_Confirmation(le)(sd) 

Sign_Confirmation(le)(xd) 

Sign_Confirmation(le)(tp) 

 

How to interpret the report:  

We can sort the percent of conversions that are cross-device (xd)/(tl) from high to low, to understand what is driving above average cross-device conversions. Our clients can use this to inform their creative or targeting strategy to match messaging and channel investment to user behavior. 

Packages - we can easily see which packages are driving the most total conversions, and which ones have a high percentage of cross-device conversions. This can help clients understand where to invest incremental budget, and improve the performance algorithm by feeding it with more data points 

Placements - compare placements to each other to see how, for example, a mobile web ad is driving conversions on desktop. Without a device graph for attribution, we may miss a mobile web placements conversion volume on desktop, or it may be downplayed if the majority of users convert on desktop and not mobile web. 
 

Ads - have a clearer picture of which creatives are driving more total conversions. If a creative is repurposed across channels, we can see if Creative A on desktop and Creative A on mobile are driving more total conversions than Creative B on desktop and Creative Creative on mobile. 
 

Sites - Traditionally, manual optimization turns sites off that are low performers. Now clients will have more confidence these optimizations are not turning off sites that were driving cross-device conversions, increasing overall conversion volume. 

Feeds - Similar to sites, ensure manual optimizations are made with better insight, as we can see if certain feeds are more prone to delivering cross-device conversions, and if we should expand our targeting to include more devices and channels in those feeds. 
 

We can also better quantify and validate investment in mobile app ads for a conversion event that occurs on a web browser, giving buyers a more complete view of their investment and opening up a large section of mobile inventory for targeting. 

For customers who are not using but are interested in implementing our Advertising Cloud Conversion pixels on their site, please connect with your Account Manager to set this up. Set up details for reference. 