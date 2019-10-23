---
edit-last: 41
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
ldc-disable: 0
ldc-disable-comm: 0
pubDate: Fri, 04 Jul 2014 16:22:09 +0000
dc-creator: hchang@adobe.com
guid: http://education.tubemogul.com/userguide/?page_id=1577
isPermaLink: false
description: 
postId: 1577
postDate: 2014-07-04 08:22:09
postDateGmt: 2014-07-04 16:22:09
commentStatus: open
pingStatus: open
postName: email-reports
status: publish
postParent: 1446
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Email Reports {#email-reports}

` `The custom`` ` `e`` ` `mail`` ` `r`` ` `eports tool gives you more flexibility and choice in the content and delivery of your`` ` `Adobe Advertising Cloud`` ` `data.`` ` `T`` ` `he custom`` ` `email`` ` `reports tool can help you delve deeper into your campaigns’ performance and customize the data you want to receive.`` ` `You can`` ` `generate scheduled reports for`` ` `email`` ` `delivery`` ` `to specified users`` ` `on a one-time, daily, weekly, or monthly basis`` ` `.`` ``
  
` `You can create your report f`` ` `rom scratch or choose from several`` ` `pre-configured`` ` `report`` ` `templates.`` ``

&nbsp;

[ ![Report Types](assets/report-types-1024x242.png)](assets/report-types.png)
&nbsp;   
**Where to find it**
  
Click on the Tools section in the navigation bar:

[ ![Where to find it](assets/where-to-find-it.png)](assets/where-to-find-it.png)

&nbsp;

From there, click on the Email Reports button on the far left side of the page:

[ ![Tools - Email Reports](assets/tools-email-reports-133x300.png)](assets/tools-email-reports.png)

&nbsp;
**`Building Your Report`** ``
`There are several options available for detailing what should be included in your report and how it should be applied.` ``   
**Filters**
  
` `Filters define the scope for your report.   There are two kinds of filters in email reports.`` ` ``` ``
* `1) Filter by Date`: * `D` `efine the timeframe for your report. You can s` `et` `dates to` `` `report` `on` `` `past events or set it up to send data for future campaigns.` ``
`The options for this filter are:` ``

* *** `Timezone`*** `:` `S` `elect from a list of` `timezones` `,` `depending on what’s appropriate for your campaign.  This could be the same` `timezone` `that you’ve set for the account (the default) or a different` `one, but` `remember to check` `the` `timezone` `when comparing` `reported metric` `s from the UI with` `` `what you’ve set for yo` `ur` `` `email reports.` ``

* *** `Previous __ days`**** `:`* `The default is 2 days. You can enter any number of days up 985 days (3 years) and receive full day reports leading up to today.  For example, if you created a one-time report on August 1st and selected “previous 2 days”, you would receive a report for July 31st and August 1st.`*** `Note`**** `: reports with length >90 days can only be delivered as a single frequency report.`* ``

* *** `Custom`**** `:`* `Selecting this option enables you to create a report for any date range starting on or after January 1, 2013 to any time in the future.  Select this option if you want to set up regular reports going to some future date, or if you have a very specific range not covered by the other two options` `.` ``*** `Note`**** `: reports`** `with lengt`** `h`** `>90 days can only be delivered as a single frequency report`** `.`** ``* ``

* *** `Last Calendar Month`**** `:`* `Selecting this option will return a report for the last calendar month through today’s date. For example, if I were to create a one-time report using this option on January 23rd, I would get a report for January 1st through the 23rd.` ``

[ ![Apply Filters](assets/apply-filters-1024x427.png)](assets/apply-filters.png)

&nbsp;
`* `2)`*` * ` `Additional Filters`:`* `` `The second type of filter is for parameters that will focus on specific data in your account. For example, if you only want to see data only on a certain advertiser, limit your report to pre-roll ads, or review activity for selected countries, you would set these values in the filters. ` `You can filter by:` `` * `Advertiser, Campaign, Placement, Ad, Ad Type, Video,`* * `Video`* * `Duration,`* * `and Country and Package.`* `` ``
`Up to` `six filters` `can be applied to a single report.` ``

[ ![Filter types](assets/filter-types.png)](assets/filter-types.png)

&nbsp;

When you create your filter, you can also specify criteria within that filter by specifying if the value you want is equal or not equal to a value. For example, if you want to see only ad types that are not pre-roll or results that are only for one campaign. Once you have entered one criterion, you can use an “and” or an “or” command to link it to other criteria. For example, if you wanted data in your report for the US and Canada, your filter would look like this:

[ ![Country Equals](assets/country-equals.png)](assets/country-equals.png)

&nbsp;

But if you want to see only data for all countries outside the US or Canada, you would set it up this way:

[ ![Country NOT Equals](assets/country-not-equals.png)](assets/country-not-equals.png)

&nbsp;

Be careful when using the “and” command with “equals” in particular when creating reports. Putting these two together can actually exclude all of the data, if you set it to equal and not equal one variable. For example, this filter would exclude all of the data:

[ ![Country Equal and NOT equals](assets/country-equal-and-not-equals.png)](assets/country-equal-and-not-equals.png)

&nbsp;
`This is telling the database to get all of the records where the c` `ountry` `is` `Australia` `but are also not` `Australia` `.` ``
`Putting this all together, if you wanted to create a report for May 1st – July 31st 201` `9` `that will only show data for advertiser` `“Example’s”` `` `video` `ads in the United States and Canada, your filters would look like this:` ``

[ ![Filter combo](assets/filter-combo.png)](assets/filter-combo.png)

&nbsp;

**Build your report**

In this section, you’ll be selecting the “meat” of your report and how it will be arranged and sliced.

[ ![Dimensions and Metrics 2](assets/dimensions-and-metrics-2.png)](assets/dimensions-and-metrics-2.png)

&nbsp;
There are two groups of items you can select here:

* ***Dimensions***:  ` `These are categories of data and tasks that we organize campaigns around, like advertiser, ad type, placement, etc. It also includes the time frames you want to look at (`` ` `eg.`` ` `hour, day, week, month, etc.) and geographic area.`` ` `These will define the rows in your report.`` ``

* ***Metrics***:  ` `These are the actual measurements of the campaign that help you determine if you hit your goals, like impressions, click-throughs, completions, etc.`` ` `These will define the columns in your`` ` `report.`` ``

* ` `***Conversion Metrics***: Advertising Cloud conversion metrics captured using multi-touch `` ` `Advertising Cloud conversion metrics`` ` `will be available if you have`` ` `configured multi-touch conversion tracking.`` ` `This will include Adobe Analytics conversions as well`` ` ``` ` `conversions`` ` `captured using`` ` `the`` ` `Advertising Cloud Conversion pixel`` ` `, depending on which kinds of tracking you have configured`` ` `.`` ` ``` ` `You will see a list of advert`` ` `isers and beneath each advertiser`` ` `,`` ` `you will see the Conversion Metrics available for`` ` `that` `particular`` ` `a`` ` `dvertiser``. To learn more about conversion optimization tactics, go [here](../new/performance-display-playbook.md).`
  
  `***Note***` ` ` `: *These metrics will be displayed based *``* ` `on the`` ` `multi-touch attribution rules you specify in the Report Options section.``*``

* ` ` `***Custom Goals***: ```These are `` `combinations for Conversion Metrics used as goals for` `Ad` `vertising` `Cloud` `s optimization eng` `ine.` `This option will be available if you have configured multi-touch conversion tracking.` `Like` `Convers` `i` `on` `Metrics you can see the Custom Goal available` `listed beneath each advertiser. To learn more about how to setup Custom Goals, go [here](../new/performance-display-playbook/building-a-custom-goal.md).` ``   
  *** `Note`**** `: These metrics will be displayed based multi-touch attribution rules you specify in the Report Options section.`* ``

To add a Dimension or Metric to your report:

1. In the box on the left, expand the relevant group and make a selection from the options.
1. In the box on the right, select the check box next to your selection.
1. In the summary below, your selection will appear.

The screenshot below shows the process for specifying you want hourly data in your report:

[ ![Selecting Dimension Metrics from list](assets/selecting-dimension-metrics-from-list.png)](assets/selecting-dimension-metrics-from-list.png)

&nbsp;
`Continue doing this until you have selected all of the dimensions and metrics you want to include` `. Note that you can drag your selections in the box at the bottom to reorder your headers in the report.` ``
`This example shows what the screen would look like for a report that will show you hourly reporting, by campaign and country on impressions and 100% video completion.` ``

[ ![CR9](assets/cr9.jpg)](assets/cr9.jpg)

**&nbsp;**

**Report Options**

*** `Format and Report Headers`*``**
`These settings determine the format in which you’d like your report to be delivered, whether CSV or tab format, include the header or remove headers, which means the name of the report and the filters applied to it, like the date range.` ``

[ ![report format](assets/report-format.png)](assets/report-format.png)

&nbsp;
`After you’ve set your format and headers` `, you can` `choose options related to multi-touch attribution. Multi-touch attribution allows you to view Conversion` `Metrics and Custom Goals in many different ways.` `For` `example,` `` `if your Conversion Metric is “Orders”` `y` `ou can choose` `to see “Orders” based on` `` `a` `specified` `attribution rule and view-through weight.` ``
*** `Note`*** * `: these options are only applicable to advertisers with multi-touch attribution enabled`* * `. To verify, check your`* [* `advertiser settings`*](https://www.tubemogul.com/adcloud/settings/profile/advertiser-list?&action=ADVERTISER_LIST_SEARCH) * `.`* * `To have your advertiser be setup for multi-touch attribution, please contact your account manager.`* ``

[ ![Report Options](assets/report-options1.png)](assets/report-options1.png)

&nbsp;
*** `Attribution Rule Settings`*** ``
`You can choose one or more attribution rules` `. Based on the rule chosen` `,` `the values for your Conversion Metrics and Custom Goals will change.` `For` `example,` `under` `“` `First` `` `event”` `att` `ribution Ad A may get credit for a conversion. Under` `“` `Last` `event”` `attribution rule Ad B may get credit.` `` `You can include multiple attribution rules for side-by-side comparison. You can learn more about how Attribution Rules are calculated [here](assets/attribution-advertising-cloud.pdf).` ``

*** `Paths as Columns`*``**
`This allows you to see` `Conversion Metrics and Custom Goals broken out based` `on` `whether they were preceded by a click or an impression.` `Or you can just see the total without any` `breakout` `.` ``
`Additionally,` `when view` `ing the` `Total` ` you can choose a view-through weight to apply. Learn more about view-through weights [here](assets/attribution-advertising-cloud.pdf).` ``
`Terminology` ``

1. `***Total (TL) = CT + VT &#42; VT weight: ***: Total conversions including view-through conversions and click-through conversions. View-based conversions will be adjusted according to the view-through weight specified. View-through weight a value between 0% and 100%. The view-through weight will default to the value you have specified for attribution settings. In the report this will be indicated with a “(TL)” after the conversion name.  ` ``

1. `***With Clicks (CT)***: Click-based conversions. These are any conversions preceded by at least one click. This is a raw value and is not adjusted according to the view-through weight. In the report this will be indicated with a “(CT)” after the conversion name.` ``

1. *** `Impression Only (VT)`***:  View-based conversions. The are conversions preceded by only impressions. In the report this will be indicated with a “(VT)” after the conversion name. ``

*** `Cross-Device Reporting`*``**
`This allows you to see Conversion Metrics and Custom Goals based` `on` `` `whether the conversion was same-device or cross-device.` `Cross-device conversions will only be measured if` `an Advertiser has been` `configur` `ed` `to use` `a device graph` `.` `` `A conversion is defined as cross-device if` `more than one device was involved in the path to conversion.` ``
`Terminology` ``

1. `***Same-Device (sd)***: Conversions where only one device was present in the conversion path. In the report, next to your conversion metric name and rule type, you will see (SD). ` ``

1. `***X-Device (sd)***: Conversions where more than one device was present in the conversion path. In the report, next to your conversion metric name and rule type, you will see (XD). ` ``

1. *** `Total` `conversions` `includ` `ing` `cross device` `- if applicable` `(tp`*** `***)***:  Total conversions including both same device and cross device (if applicable).` `` `In the report, next to your conversion metric name and rule type, you will see (tp).` ``

*** `Note`*** * `: cross-device options are only applicable to advertisers with cross-device enabled.`* * `If you do not have a device graph enabled for a specific adv`* * `ertiser, then your`* * ``* * `(xd) column will not contain any values and your (sd) and (tp) values will be the same.`* * ``* * `Cross device attribution reporting is free of charge and one attribution graph can be mapped to a single advertiser.`* ``
`` * `To verify if your advertiser has cross device enabled, check your  [advertiser settings](https://www.tubemogul.com/adcloud/settings/profile/advertiser-list?&action=ADVERTISER_LIST_SEARCH)`* * ` [page](https://www.tubemogul.com/adcloud/settings/profile/advertiser-list?&action=ADVERTISER_LIST_SEARCH) `* * `under General > Integrations > “Cross-device attribution”`* * `.`* * `To have your advertiser be setup for cross-device, please contact your account manager.`* ``

*** `C`** `onversion`** `Reporting Based On`*``**
`This affects the date` `see Conversion Metrics and Custom Goals are associated with.` `“Conversion Timestamp” will show values based` `on the day the conversion event happened.` `“Event Timestamp” will show values based on the day the impression or click happened.` ``

&nbsp;

**`Combinations`**
`The report will automatically include all combinations of the` `attribution options you have chosen.` `The column label will` `include` `` `values` `indicat` `ing which options apply to that metr` `i` `c.` ``
`For` `example` `,` `if you choose t` `he following options` `…` ``

[ ![Combo](assets/combo.png)](assets/combo.png)

&nbsp;
` `…you will`` ` `see t`` ` `wo different columns for each of you Conversion Metrics. If you`` ` `h` `ad` `chosen “orders” as a conversions metric your report would include these columns.``
&nbsp;   
**Add Email Recipients**
  
`In this section, you can specify who you’d like to receive the report, and how frequently. Reports can be sent` `multiple email addresses and each r` `ecipient can be set to have their report delivered at a` `specific interval:` `a one-time, daily, weekly or monthly basis.` ``
`* `Reminder`*` `: in order to deliver a report >90 days,` `only` `report` `s with a delivery frequency of “once”` `allow for it.` ``
`When you’re ready to s` `chedule or send the report, click on` `“Create Custom Report.” By creating your report,` `you are also saving it and thus` `can always return and edit your report settings` `later.` ``

[ ![Email Run NOw](assets/email-run-now.png)](assets/email-run-now.png)

&nbsp;
` `Scheduled reports`` ` `will be delivered to the addresses you specify at about 9 am the next morning according to the` `timezone` `specified in the request as a link to a page where they can download the file.  They will look like this:`` ``

[ ![CR12](assets/cr12.jpg)](assets/cr12.jpg)

&nbsp;

**Editing and deleting your reports**

If you ever need to change or edit your reports, simply go to the “Email Reports” page, and click on the options link.

[ ![Edit Reports](assets/edit-reports.png)](assets/edit-reports.png)

&nbsp;
If you have any additional questions feel free to reach out the Platform Strategy team at ` ` `` [ ` ` `platform_support@`` ` `Adobe Advertising Cloud`` ` `.com```](assets/ platform-support@adobe%20advertising%20cloud.com).

&nbsp;
&nbsp; 