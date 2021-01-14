---
title: Duplicate Placements
description: Duplicate Placements
---

# Duplicate Placements

<!-- Some placements don't have this option. Clarify which placement types aren't eligible -- is it PG and simple ad serving placements, or all placements using private inventory? And anything else? -->

Duplicate one or more placements to create placements with similar settings. You can:

* Make multiple duplicates of placements
* Duplicate placements within the original advertisers and campaigns or within different ones
* (For duplicated placements within the original campaigns) Optionally duplicate the original ads
* Modify the status and flight dates of the new placements

All settings from the original placements are duplicated except:

* Experiment settings
* (If you change the flight dates) Custom ad scheduling
* (If you don't attach ads) Custom ad weighting and scheduling
* Programmatic guaranteed (PG) default placements and Simple Ad Serving placements
* (Placements copied to a different campaign):
    * Geo targets
    * Event pixels
    * Ads
    * <!-- Placement-level? This said "custom," so verify if that means placement-level as opposed to advertiser-level segments -->DoubleVerify Authentic Brand Safety segments

1. In the main menu, click **Campaigns**.
1. Click the name of the campaign.
1. In the submenu, click **Placements**.
1. Do either of the following:
    * To duplicate one placement, click  **... > Duplicate** next to the package name.
    * To duplicate multiple placements:
        1. Select the check box next to each placement to duplicate.
        1. In the bulk actions toolbar, click **Duplicate**.
1. Specify the new placement settings:
    1. (Single placements) Enter the new placement name.
    1. In the **Choose Package (Required)** menu, select either the parent package or **No package*.
    1. (Optional) Change the default settings.
    
    The settings apply to all selected placements.

    By default, the new placements are for the original ad type, are assigned to the original advertisers and campaigns, have flight schedules that begin on the current day, are paused, and don't include the original ads.

    When you create multiple placements, the new placement names are appended with a number, in sequence, using the convention <*original_placement_name #N*>, such as "My Placement #2."

1. Click **Submit**.

>[!MORELIKETHIS]
>
>* [About Placement Management](placement-about.md)
>* [Create a Placement](placement-create.md)
>* [Edit a Placement](placement-edit.md)
>* [Placement Settings](placement-settings.md)
