---
title: Duplicate a Campaign
description: Duplicate a Campaign
---

# Duplicate a Campaign

<!-- Some placements don't have this option. Clarify which placement types aren't eligible -- is it PG and simple ad serving placements, or all placements using private inventory? And anything else? -->

Duplicate a campaign to create a new campaign with similar settings. You can:

* Duplicate the campaign for the original advertiser or for a different one
* Optionally duplicate the original packages and placements
* Modify the flight dates of the new campaign

See "[What's Not Duplicated](#campaign-not-duplicated)" for a list of placement settings that aren't duplicated.

1. In the main menu, click **Campaigns**.
1. Next to the campaign name, click  **... > Duplicate**.
1. Specify the new campaign settings:
    1. Enter the new campaign name and the end flight date.
    1. (Optional) Change the default settings.

         By default, the new campaign is assigned to the original advertiser, has a flight schedule that begins on the current day, and includes the original packages and placements.

1. Click **Submit**.

## What's Not Duplicated {#campaign-not-duplicated}

All settings from the original placements are duplicated except:

* Experiment settings
* (If you change the flight dates) Custom ad scheduling
* (If you don't attach ads) Custom ad weighting and scheduling
* Programmatic guaranteed (PG) default placements and Simple Ad Serving placements
* (If you copy placements to a different campaign):
    * Geo targets
    * Event pixels
    * Ads
    * Placement-level DoubleVerify Authentic Brand Safety segments (which override the advertiser-level segments)

>[!MORELIKETHIS]
>
>* [About Campaign Management](campaign-about.md)
>* [Create a Campaign](campaign-create.md)
>* [Edit a Campaign](campaign-edit.md)
>* [Campaign Settings](campaign-settings.md)
