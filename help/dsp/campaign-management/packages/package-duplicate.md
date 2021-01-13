---
title: Duplicate a Package
description: Duplicate a Package
---

# Duplicate a Package

Duplicate a package to create a package with similar settings. You can:

* Duplicate the package within the original advertiser and campaign or within different ones
* Optionally duplicate the placements within the package
* (For duplicated packages within the original campaigns) Optionally duplicate the original ads and placement-level event pixels
* Modify the flight dates of the new package

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
1. Click the name of the campaign to open the Packages view.
1. Next to the package name, click  **... > Duplicate**.
1. Specify the new package settings:
    1. Enter the new package name.
    1. (Optional) Change the default settings.
    
         By default:
         
         * The new package is assigned to the original advertiser and campaign.
         * The new package becomes active on the current day.<!-- and the flight continues for NN  days. -->
         * Placements within the original package are copied to the new package.
         * The ads and the placement-level event pixels aren't copied to the new package.
1. Click **Save**.

>[!MORELIKETHIS]
>
>* [About Package Management](package-about.md)
>* [Create a Package](package-create.md)
>* [Edit a Package](package-edit.md)
>* [Package Settings](package-settings.md)
