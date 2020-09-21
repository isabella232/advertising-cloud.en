---
title: Brand Safety and Media Quality
description: Brand Safety and Media Quality
---

# Brand Safety and Media Quality

<!-- Check on logo sizes in staging environment -- I made them all 100 pixels high except for DoubleVerify, which is 150 (harder to see at 100), but some instances look larger in VS Code. -->

Advertising Cloud DSP provides a suite of brand protection features to ensure that each of your campaigns reaches real users in a brand-safe environment.

Our Fraud Surveillance team works closely with industry leading partners, such as the Interactive Advertising Bureau, Trust and Accountability Group, and WhiteOps, to carefully curate the inventory on our platform. Through proactive management of our supply, DSP ensures that all advertisers across the platform are protected from non-human traffic (bots, crawlers, datacenter traffic, and fraud) and deliver only in brand-safe contexts.

In addition to providing central quality management, we believe in empowering advertisers to design the controls that align with their brand. Adobe Advertising Cloud offers integrations with Comscore, DoubleVerify, Integral Ad Science, Oracle Data Cloud, and Peer39, ensuring that each advertiser can choose their desired level of fraud protection, contextual filtering, and keyword targeting.

## Advertising Cloud DSP Quality Initiatives

### Inventory Verification with Ads.txt Support

[Ads.txt](https://iabtechlab.com/ads-txt) (Authorized Digital Sellers) is an initiative launched by IAB in June 2017 to facilitate the proper representation of inventory on the open market, thereby combatting illegitimate sources of traffic and domain spoofing. Participating publishers and distributors publicly declare the companies authorized to sell their digital inventory, and the nature of those relationships, by maintaining an ads.txt page at the top level of the domain (such as example.com/ads.txt).

DSP supports ads.txt by reading each publisher's ads.txt file and giving you the option to purchase only from verified ads.txt sellers. For example, by matching the sellers we see accessing nytimes.com to the New York Times' ads.txt file, we can identify which are legitimate and which are not, and we'll block the offenders if the placement is configured to purchase only from verified sellers. <!-- can we actually mention NY Times? -->

You can set default ads.txt controls for each advertiser<!-- [default ads.txt controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, and then optionally [customize the settings for each placement](/help/dsp/campaign-management/placements/placement-settings.md) to:

* buy inventory from a domain's authorized direct sellers only

* buy inventory from a domain's authorized direct sellers and resellers only

* prioritize buying inventory from a domain's authorized direct sellers and resellers

* buy inventory from all sellers

### Platform Fraud Surveillance

DSP has built strong internal tools and systems to manage fraud across our platform, partnering with leading industry vendors such as Whiteops and Integral Ad Science.

In addition, Adobe works closely with the Interactive Advertising Bureau (IAB) and the Trust and Accountability Group (TAG) to ensure robust, industry-standard fraud blocking to protect our advertisers, leveraging tools such as ads.txt (see the previous section), IAB's Bots and Spiders list, and TAG’s Datacenter IP list.

Through our multi-dimensional approach to quality, our team monitors anomalies and invalid traffic patterns, ensuring less than 3% invalid traffic on protected inventory. Any inventory that is suspicious &mdash; including inventory on specific domains or from specific publishers or sellers &mdash; is immediately blocked across the platform.

### Inventory Mapping, Tiering, and Categorization

Inventory mapping is the detailed review and on-boarding process required for all new inventory before it's added to our platform. This process is designed to ensure the safety and quality of all inventory on DSP.

* **Mapping:** Our Inventory team reviews each domain carefully, evaluating aspects such as:

   * Brand safety

   * Ad type verification
 
   * Generic content, duplicate domains, and fake ad serving

* **Tiering:** We holistically examine brand presence in the overall ecosystem to classify inventory across different tiers. You can [target your placements](/help/dsp/campaign-management/placements/placement-settings.md) to these tiers for the desired level of reach:

   * **T1** – Brand-name, internationally-recognizable sites

   * **T2** – Great-looking sites that are current, up-to-date, without user-generated content, and usually lacking in global recognition

   * **T3** – User-generated content and niche content

* **Site categorization:** To ensure easy content targeting and blocking, we tag each property with an Advertising Cloud-defined site category based on the property's content. You can [target or exclude these site categories for each placement](/help/dsp/campaign-management/placements/placement-settings.md) based on the placement goals.

### Comprehensive Support for Site Blocking

Advertising Cloud DSP provides both a globally blocked sites list and the option to create custom blocked sites lists for advertisers and accounts.

#### Advertising Cloud DSP Globally Blocked Sites List

Advertising Cloud DSP maintains a globally blocked sites list of sites deemed unsafe to run ads on. This list contains sites featuring objectionable content (such as hate or terror) and sites infected by bots, fake pre-roll, mismatched domains, and other fraudulent activity.

As part of our Brand Safety initiative to root out activities that defraud advertisers, all sites are screened using the measures in the chart blocked sites list. All sites that don't pass the brand safety checks are added to the globally blocked sites list. Because Advertising Cloud DSP manages this list dynamically, sites may move on or off the list at any time, based on the latest brand safety analysis.

When you include a site on the globally blocked sites list as a placement target, the site is flagged with a red exclamation point (!). This indicates that ads will not run on the flagged site.

#### Account-level and Advertiser-level Blocked Sites Lists

Users can also maintain account-level and advertiser-level blocked sites lists<!-- [account-level and advertiser-level blocked sites lists](/help/dsp/admin/blocked-sites-list-edit.md) -->, which are used automatically for all placements. Lower-level blocked sites list are applied in addition to the globally blocked sites list.

## Third-party Integrations

### Contextual Filtering

Contextual filtering allows you to target or block ad opportunities based on the context of the page on which the ad would serve. Adobe provides contextual filtering via integrations with leading vendors in the industry: Comscore, DoubleVerify, Integral Ad Science, and Peer39. Examples of current filters include Adult Content, Natural Disasters, Legal Drinking Age, MANGA, Epidemics, and G-rated Sites.

You can set default contextual filter controls for each advertiser<!-- [default contextual filter controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, and then optionally [customize the settings for each placement](/help/dsp/campaign-management/placements/placement-settings.md). Additional fees may apply when you use this feature.

<table >
    <tr>
        <td><p><img src="../../assets/comscore-logo.png" title="Comscore logo" alt="Comscore logo" style="border: none;" border="0" /></p></td>
        <td><p><img src="../../assets/doubleverify-logo.png" title="DoubleVerify logo" alt="DoubleVerify logo" style="border: none;" border="0" /></p></td>
        <td><p><img src="../../assets/ias-logo.png" title="Integral Ad Science logo" alt="Integral Ad Science logo" style="border: none;" border="0" /></p></td>
        <td><p><img src="../../assets/peer39-logo.png" title="Peer39 logo" alt="Peer39 logo" style="border: none;" border="0" /></p></td>
    </tr>
</table>

<!-- ![Comscore logo](/help/dsp/assets/comscore-logo.png) ![DoubleVerify logo](/help/dsp/assets/doubleverify-logo.png) ![Integral Ad Science logo](/help/dsp/assets/ias-logo.png) ![Peer39 logo](/help/dsp/assets/peer39-logo.png) -->

### Pre-Bid Fraud Blocking

Leverage our third-party integrations with Comscore, DoubleVerify, Integral Ad Science, and Peer39 to block non-human traffic from your campaigns. These integrations provide industry-leading pre-bid blocking capabilities to minimize both general and sophisticated invalid traffic (GIVT and SIVT) in your campaigns.

You can set default pre-bid fraud blocking controls for each advertiser<!-- [default pre-bid fraud blocking controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, and then optionally [customize the settings for each placement](/help/dsp/campaign-management/placements/placement-settings.md). Additional fees may apply when you use this feature.

For more information on functionality, contact your preferred vendor directly, or contact your Adobe account manager.

<table >
    <tr>
        <td><p><img src="../../assets/comscore-logo.png" title="Comscore logo" alt="Comscore logo" style="border: none;" border="0" /></p></td>
        <td><p><img src="../../assets/doubleverify-logo.png" title="DoubleVerify logo" alt="DoubleVerify logo" style="border: none;" border="0" /></p></td>
        <td><p><img src="../../assets/ias-logo.png" title="Integral Ad Science logo" alt="Integral Ad Science logo" style="border: none;" border="0" /></p></td>
        <td><p><img src="../../assets/peer39-logo.png" title="Peer39 logo" alt="Peer39 logo" style="border: none;" border="0" /></p></td>
    </tr>
</table>

### Topic Targeting

DSP topic targeting allows you to target or block keyword lists by leveraging our industry-leading contextual partners Comscore and Oracle Data Cloud (Grapeshot).
Topic targeting helps you to ensure your ads are always served in an environment that aligns with your brand, whether that includes blocking harmful content or ensuring spend in a context that ensures a greater outcome.

Topic targeting requires you to create topic segments directly with Comscore or Grapeshot (using Oracle Data Cloud). Once these are created in the partner platform, you can [target or exclude a segment ID in the Audience Targeting section for each placement](/help/dsp/campaign-management/placements/placement-settings.md). Additional fees may apply for this feature.

To get started, contact your preferred vendor or your Adobe account manager.

<table >
    <tr>
        <td><p><img src="../../assets/comscore-logo.png" title="Comscore logo" alt="Comscore logo" style="border: none;" height="100" width="618" border="0" /></p></td>
        <td style="height:100px"><p><img src="../../assets/oracle-grapeshot-logo.png" title="Grapeshot logo" alt="Grapeshot logo" style="border: none;" height="100" width="171" border="0" /></p></td>
    </tr>
</table>

### DoubleVerify Authentic Brand Safety

DSP has partnered with DoubleVerify to offer its Authentic Brand Safety targeting solution, which allows you to create a centralized set of brand safety requirements to target across all of your buying platforms for consistency.

Once you have built a DoubleVerify brand safety segment with the necessary targeting, you can use it within DSP to replicate your post-bid block rules with pre-bid across web environments.

You can specify a DoubleVerify segment ID for each advertiser<!-- [specify a DoubleVerify segment ID for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, and then optionally [enable or disable Authentic Brand Safety for each placement](/help/dsp/campaign-management/placements/placement-settings.md). DSP bills your account for usage for the segment ID.

For more information about functionality, contact DoubleVerify directly, or contact your Adobe account manager.

<table >
    <tr>
        <td><p><img src="../../assets/doubleverify-logo.png" title="DoubleVerify logo" alt="DoubleVerify logo" style="border: none;" height-="150" width="158" border="0" /></p></td>
    </tr>
</table>

>[!MORELIKETHIS]
>
<!-- >* [Advertiser Account Settings](/help/dsp/admin/advertiser-settings.md) -->
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
