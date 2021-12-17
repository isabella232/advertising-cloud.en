---
type: Documentation
cloud: Experience Cloud
solution: Advertising Cloud
product: advertising cloud
title: About Account-level and Advertiser-level Blocked Sites Lists
description: About Account-level and Advertiser-level Blocked Sites Lists
---

# About Account-level and Advertiser-level Blocked Sites Lists

<!-- Can you just add domains for your acct profile or advertiser to which you have access? It doesn't look like you can remove or edit any existing domains. Or can you with a specific syntax? -->

<!-- For domains, sub-domains,...? Specify what is valid. -->
You can edit the blocked sites list used for the entire Advertising Cloud account and additional lists for individual advertisers in the account.

Blocked sites lists define sets of targets to exclude for your placements. Each list can consist of top-level website domains and any level <!--- verify --> of sub-domains (such as example.com, my.example.com, or my.new.example.com)) and mobile app names (such as ???)<!-- package names/app IDs, the full URL in Google Play/iTunes? Specify what is valid. -->.

Advertiser-level lists override account-level lists.

>[!NOTE]
>
>* Account-level and advertiser-level blocked site lists are applied in addition to the Advertising Cloud DSP [globally blocked site list](/help/dsp/introduction/features/brand-safety-media-quality.md), which include sites deemed unsafe for ads.
>* Users can also add targeted sites to any placement.
>* Blocked sites lists always override targeted sites lists. If a placement both excludes and includes the same target for an ad, then the target is excluded. <!-- Verify -->

>[!MORELIKETHIS]
>
<!--
>* [Edit an Account-level or Advertiser-level Blocked Site List](/help/dsp/admin/blocked-sites-list-edit.md)
[Brand Safety and Media Quality](/help/dsp/introduction/features/brand-safety-media-quality.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
-->
