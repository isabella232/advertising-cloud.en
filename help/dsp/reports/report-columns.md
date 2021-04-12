---
type: Documentation
cloud: Experience Cloud
solution: Advertising Cloud
product: advertising cloud
title: Available Report Columns
description: Available Report Columns
exl-id: c96e46ae-2fb2-4364-9c51-f160c00693ba
---
# Available Report Columns

|Metric Type|Subtype|Column Name|Description|
|-----------|-------|-----------|-----------|
|Dimension|Ad|Ad External ID|The ad ID assigned by the external ad server.|
|Dimension|Ad|Ad ID|The unique identifier for the ad in Advertising Cloud.|
|Dimension|Ad|Ad Name|The name of the ad as assigned by the user.|
|Dimension|Ad|Ad Type|The format of the ad.|
|Dimension|Ad|Status|The classification of the ad as altered by the user or denoted by the date inputs: *live*, *scheduled*, *completed*, or *archived*.|
|Dimension|Advertiser|Advertiser Name|The name of the advertiser.|
|Dimension|Campaign|Budget|The total budget assigned by the user for the campaign.|
|Dimension|Campaign|Campaign End Date|The end date for the campaign.|
|Dimension|Campaign|Campaign ID|The unique identifier for the campaign in Advertising Cloud.|
|Dimension|Campaign|Campaign Name|The name of the campaign as assigned by the user.|
|Dimension|Campaign|Campaign Start Date|The first date for the campaign.|
|Dimension|Date/Time|Day (YYYY-MM-DD)|The year, month, and day.|
|Dimension|Date/Time|Day of Week|The specific day, such as Monday or Tuesday.|
|Dimension|Date/Time|Hour (YYYY-MM-DD HH)|The year, month, day, and hour.|
|Dimension|Date/Time|Month (YYYY-MM)|The month and year.|
|Dimension|Date/Time|Time of Day|The time to the hour, from 0-23.|
|Dimension|Date/Time|Week (YYYY-MM-DD to YYYY-MM-DD)|The date range for the relevant week, from Sunday to Saturday. Example: 2021-02-18 to 2021-03-07.|
|Dimension|Device|Browser Vendor|The vendor of the browser in which the ad was shown (such as Google or Mozilla).|
|Dimension|Device|Browser Version|The version of the browser in which the ad was shown (such as Safari 4.3 or Chrome 7.0).|
|Dimension|Device|Browser|The browser in which the ad was shown (such as Chrome or Firefox).|
|Dimension|Device|Environment|Whether the ad was shown on  *sites* or *Apps*.|
|Dimension|Device|Hardware|The type of device on which the ad was shown (such as Set Top Box or Mobile Phone).|
|Dimension|Device|Manufacturer|The manufacturer of the device on which the ad was shown (such as Samsung, Lenovo, or Apple).|
|Dimension|Device|Model|The model of the device on which the ad was shown (such as iPhone XS or Galaxy Note 7).|
|Dimension|Device|Operating System Vendor|The vendor of the operating system on which the ad was shown (such as Microsoft or Apple).|
|Dimension|Device|Operating System Version|The version of the operating system on which the ad was shown (such as Windows 10, iOS Mojave)|
|Dimension|Device|Operating System|The operating system on which the ad was shown (such as Apple iOS or Android).|
|Dimension|Feed|Deal ID|The unique identifier assigned to a deal through the external supply partner.|
|Dimension|Feed|Feed Name|The user-assigned name for the deal, as entered in Advertising Cloud.|
|Dimension|Feed|Feed Source|The supply-side partner providing the inventory. This is typically a publisher but can also be an SSP.|
|Dimension|Feed|Inventory Type|The classification of the inventory: *Private,* *On Demand,* or *Public*.|
|Dimension|Feed|SSP|The supply-side partner (SSP) to which the media is attributed.|
|Dimension|Frequency|Frequency|The number of times a device has received an ad, based on the unique cookie or device ID.|
|Dimension|Geos|City|The city to which the reported data is attributed.|
|Dimension|Geos|Country|The country to which the reported data is attributed.|
|Dimension|Geos|DMA|The Designated Market Area (DMA) to which the reported data is attributed.|
|Dimension|Geos|State|The state to which the reported data is attributed.|
|Dimension|Packages|Package End Date|The end date for the package.|
|Dimension|Packages|Package Goal Type|The pacing goal amount for the package. This amount is in either spend or impressions.|
|Dimension|Packages|Package ID|The unique identifier for the package in Advertising Cloud.|
|Dimension|Packages|Package Name|The name of the package|
|Dimension|Packages|Package Start Date|The package start date.|
|Dimension|Packages|Placement End Date|The placement end date.|
|Dimension|Pixel|Conversion ID|(Deprecated) The Conversion ID assigned by DSP to legacy TubeMogul conversion events.|
|Dimension|Pixel|Conversion Name|(Deprecated) The conversion name assigned to legacy TubeMogul conversion events.|
|Dimension|Placement|Placement ID|The unique identifier for the placement in Advertising Cloud.|
|Dimension|Placement|Placement Name|The name of the placement as assigned by the user.|
|Dimension|Placement|Placement End Date|The placement end date.|
|Dimension|Placement|Placement Start Date|The placement start date.|
|Dimension|Placement|Placement Tags|The placement tag used as a custom identifier for the placement.|
|Dimension|Segment|Billing Segment Description|The description associated with a billable segment.|
|Dimension|Segment|Billing Segment Key|The unique key associated with a billable segment.|
|Dimension|Segment|Billing Segment Name|The name of a billable segment.|
|Dimension|Segment|Segment Membership Description|The description associated with a segment, provided by the data provider.|
|Dimension|Segment|Segment Membership Key|The unique key associated with a segment.|
|Dimension|Segment|Segment Membership Name|The name of a segment.|
|Dimension|Segment|Segment Membership Provider Name|The name of the data provider associated with a segment.|
|Dimension|Site|Site ID|The unique identifier for the site or app in Advertising Cloud.|
|Dimension|Site|Site Name|The name of the site.|
|Dimension|Standard Metrics|Avg. Player Width x Height|The average player width and height.|
|Dimension|Standard Metrics|Connection|The type of internet connection that was used to view the ad (such as Wifi or 4g LTE).|
|Dimension|Video|Video Duration|The video length, which is processed after upload.|
|Dimension|Video|Video ID|The unique identifier for the video creative in Advertising Cloud.|
|Dimension|Video|Video Name|The name of the creative assigned by the user.|
|Metric|Frequency|% Distinct Uniques|The App/Site Distinct Uniques divided by App/Site Uniques.|
|Metric|Frequency|App/Site Distinct Uniques|The total number of devices that were reached on this app only. A viewer exposed to an ad across multiple publishers isn't included in this value.|
|Metric|Frequency|Cost per Distinct Unique|The total Spend divided by App/Site Distinct Uniques.|
|Metric|Frequency|Cost per Unique|The total Spend divided by App/Site Uniques.|
|Metric|Frequency|Estimated % Reached|The estimated percentage of the targeted household universe that received an exposure.|
|Metric|Frequency|Estimated Average Frequency|The average number of impressions shown to uniques. For some inventory, publishers don't pass along a device identifier, and those impressions aren't included in this value. There is a similar metric in the Frequency (by App/Site) Report, but that metric isn't estimated.|
|Metric|Frequency|Estimated Impressions (Device/Browser)|(Included in the Frequency (by Impression) report) The estimated impressions for a given frequency breakout. Advertising Cloud estimates are based on a sample of impressions. For some inventory, publishers don't pass along a device identifier, and those impressions aren't included in this value. There is a similar metric in Frequency (by App/Site) Report, but that metric isn't estimated.|
|Metric|Frequency|Estimated Uniques (Device/Browser)|(Included in the Frequency (by Impression) report) The number of unique browsers or devices recorded for a given frequency. Advertising Cloud estimates are based on a sample of impressions. For some inventory, don't pass along a device identifier, and those impressions aren't included in this value. There is a similar metric in Frequency (by App/Site) Report, but that metric isn't estimated.|
|Metric|Frequency|Estimated Universe|The sum of unique households that DSP (auctions) has seen within the date range.|
|Metric|Frequency|Extended Impressions|The total number of impressions served as a result of using a device graph for people-based, cross-device targeting.|
|Metric|Performance|Gross CPA|The average gross cost per acquisition, calculated by Gross spend / Custom Goal.|
|Metric|Performance|Gross CPC|The average gross cost per ad click, calculated by Gross Spend / Ad clicks.|
|Metric|Performance|Gross CPCV|The average cost per completed video view, calculated by Gross spend / 100% Completions.|
|Metric|Performance|Gross CPM|The average cost per 1000 impressions, calculated by Gross spend / Impressions x 1000.|
|Metric|Performance|Gross CPV|The average cost per video view, calculated by Gross spend / Views.|
|Metric|Performance|Gross vCPM|The average cost per 1000 viewable impressions, calculated by Gross spend / Viewable Impressions x 1000.|
|Metric|Performance|Net CPC|The average net cost per ad click, calculated by Net Spend / Ad clicks.|
|Metric|Performance|Net CPCV|The average net cost per completed video view, calculated by Net Spend / 100% completions|
|Metric|Performance|Net CPM|The average net cost per 1000 impressions, calculated by Net spend / Impressions x 1000.|
|Metric|Performance|Net CPV|The average net cost per video view, calculated by Net Spend / Views.|
|Metric|Performance|The total Data eCPM|The average net data cost per 1000 impressions, calculated by Net spend (Data) / Impressions x 1000.|
|Metric|Performance|The total Media CPM|The average net media cost per 1000 impressions, calculated by Net spend (Media) / Impressions x 1000.|
|Metric|Performance|The total Other eCPM|The average net cost per 1000 impressions for other fees, calculated by Net spend (Other) / Impressions x 1000.|
|Metric|Spend|Billable Data Net Spend|The total net cost of audience segment data fees billed through Advertising Cloud.|
|Metric|Spend|Billable Media Net Spend|The total net cost of billable media, including the tech fee, billed through Advertising Cloud.|
|Metric|Spend|Billable Other Net Spend|The total cost of other service fees (third-party verification partners, ad serving, and so on) billed through Advertising Cloud|
|Metric|Spend|Estimated Tax on Data|The estimated tax on third-party audience segments and data services.|
|Metric|Spend|Estimated Tax on Media|The estimated tax on media inclusive of tax applied to media cost rebilling and tech fee services in Advertising Cloud.|
|Metric|Spend|Estimated Tax on Other|The estimated tax on other service fees (inclusive of third-party verification partners, topic targeting, and so on) billed through Advertising Cloud.|
|Metric|Spend|Margin %|(When margin management is activated) The margin percentage, which is calculated by (Gross Spend - Net Spend) / Gross Spend.|
|Metric|Spend|Media Cost|The sum of Non-billable and Billable media cost without tech fee|
|Metric|Spend|Net vCPM|The average net cost per 1000 viewable impressions, calculated by Net spend / Viewable Impressions x 1000.|
|Metric|Spend|Non-Billable Data Net Spend|The total net cost of audience segment data fees not billed through Advertising Cloud.|
|Metric|Spend|Non-Billable Media Fees|The total net cost of non-billable media, including the tech fee, not billed through Advertising Cloud|
|Metric|Spend|Non-Billable Other Net Spend|The total cost of other service fees (third-party verification partners, ad serving, and so on) not billed through Advertising Cloud.|
|Metric|Spend|Profit|Gross Spend - Net Spend|
|Metric|Spend|The total Data Net Spend|The total net cost of audience segment data fees.|
|Metric|Spend|The total Media Net Spend|The total net cost of media, including tech fees.|
|Metric|Spend|The total Net Spend|The sum of Net spend (Media), Net spend (Data), and Net spend (Other).|
|Metric|Spend|The total Non-Billable Net Spend|The sum of Non-billable spend (Media), Non-billable spend (Data) and Non-billable spend (Other).|
|Metric|Spend|The total Other Net Spend|The total net cost of other service fees (third-party verification partners, ad serving, and so on).|
|Metric|Spend|The total Billable Net Spend|The sum of Billable spend (Media), Billable spend (Data) and Billable spend (Other).|
|Metric|Standard Metrics|100% Completion Rate|The percentage of views that watched the ad in its entirety.|
|Metric|Standard Metrics|100% Completions|The number of views that watched the ad in its entirety.|
|Metric|Standard Metrics|100% Viewable Completion (%)|The percentage of viewable impressions that watched the ad in its entirety.|
|Metric|Standard Metrics|25% Completion Rate|The percentage of views that watched at least one quartile of the ad.|
|Metric|Standard Metrics|25% Completions|The number of views that watched at least one quartile of the ad.|
|Metric|Standard Metrics|50% Completion Rate|The percentage of views that watched at least two quartiles of the ad.|
|Metric|Standard Metrics|50% Completions|The number of views that watched at least two quartiles of the ad.|
|Metric|Standard Metrics|50% Viewable Completion (%)|The percentage of viewable impressions that watched at least two quartiles of the ad.|
|Metric|Standard Metrics|75% Completion Rate|The percentage of views that watched at least three quartiles of the ad.|
|Metric|Standard Metrics|75% Completions|The number of views that watched at least three quartiles of the ad.|
|Metric|Standard Metrics|Avg Percent Viewed|The average percentage an ad was watched to completion, accounting for all views.|
|Metric|Standard Metrics|Banner and Overlay Clicks|The number of clicks on the ad overlay and banners.|
|Metric|Standard Metrics|Click Through Rate|The percentage of clicks divided by ad impressions.|
|Metric|Standard Metrics|Clicks Per View Rate|The percentage of clicks divided by video views.|
|Metric|Standard Metrics|Companion Clicks|The number of companion banner clicks.|
|Metric|Standard Metrics|Companion CTR|The percentage of clicks divided by companion banner impressions.|
|Metric|Standard Metrics|Companion Impressions|The number of companion banner impressions.|
|Metric|Standard Metrics|Engagements|The number of interactions on a served ad.|
|Metric|Standard Metrics|Impressions|The total number of ad impressions.|
|Metric|Standard Metrics|Play Rate|The percentage of impressions served that resulted in video views.|
|Metric|Standard Metrics|Playtime per View|The average duration of a video view, measured in seconds.|
|Metric|Standard Metrics|The total Ad Clicks|The sum of all clicks on an ad.|
|Metric|Standard Metrics|Viewed Minutes|The total number of minutes a video ad was viewed.|
|Metric|Standard Metrics|Views|The total number of video ad views.|
|Metric|Viewability|Measurable Impressions|The total number of impressions served that were able to be measured for viewability.|
|Metric|Viewability|Measurable Rate (%)|The percentage of impressions served that were able to be measured for viewability, calculated as Measurable impressions x 1000 /Impressions.|
|Metric|Viewability|Unmeasurable - iFrame (%)|The percentage of impressions not measurable for viewability due to incompatible iFrames.|
|Metric|Viewability|Unmeasurable - Not Supported (%)|The number of impressions not measurable for viewability due to unsupported viewability tracking on the ad unit.|
|Metric|Viewability|Unmeasurable - Other (%)|The percentage of impressions not measurable for viewability due to other reasons.|
|Metric|Viewability|Unmeasurable Impressions|The number of ad impressions not measurable for viewability.|
|Metric|Viewability|Unmeasurable Rate (%)|The percentage of ad impressions not measurable for viewability.|
|Metric|Viewability|Unmeasurable rate (Not supported)|The percentage of impressions not measurable for viewability due to unsupported viewability tracking on this ad unit.|
|Metric|Viewability|Viewability Rate (%)|The percentage of viewable impressions out of all measurable impressions, calculated as Viewable Impressions / Measurable Impressions.|
|Metric|Viewability|Viewable Impressions|The number of ad impressions considered viewable.|
|Conversions|[Grouped by advertiser in report settings]|[Advertiser-specific conversion]| The total for a specified advertiser-specific conversion metric or Adobe Analytics event.|
|Custom Goals|[Grouped by advertiser in report settings]|[Advertiser-specific custom goal]|The weighted sum of all conversions that are included in the specified [custom goal](/help/dsp/optimization/custom-goal-about.md).|

<!-- |Omitted|Performance|Custom Goal CPA|The average cost per acquisition, calculated by Gross Spend / Custom Goal| -->
<!-- |Omitted|Performance|Custom Goal ROAS|The average return on ad spend, calculated by Custom goal / Gross spend|-->

>[!MORELIKETHIS]
>
>* [About Custom Reports](/help/dsp/reports/report-about.md)
>* [Create a Custom Report](/help/dsp/reports/report-create.md)
>* [Custom Report Settings](/help/dsp/reports/report-settings.md)
