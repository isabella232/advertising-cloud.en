---
title: Create a Reusable Audience
description: Create a Reusable Audience
---

# Create a Reusable Audience

<!-- "Saved audience" is used in UI, but "saved" is a state, not a type. "Reusable audience" sounds better in a description. "Audience template" isn't perfect, either, since it implies you can edit it on the fly to create a new, different audience. Some other term? -->

You can save and manage reusable audiences, which are groups of audience segments and even other saved audiences, which you can use as targets or exclusions for multiple placements.

1. In the main menu, click **Audiences > All Audiences**.

1. Above the data table, click **Create**.

1. Enter a unique Audience Name.

1. (Optional) Deselect the option to **Share with all advertisers in my account**.

   When you share an audience, the audience becomes available as a target or exclusion to all advertisers within the account. However, the individual segments in the audience are available only to users to which the segments are shared. For example, if you share an audience containing Adobe Analytics segments with an advertiser who is not mapped to the same Analytics account, then the segment will not preview in that audience for that advertiser. Only the segments available to that advertiser will preview in the audience.

1. Click **Save**.

1. Build the audience:

   >[!NOTE]
   >
   >As you build the audience, detailed [audience size data](audience-about.md) is updated in the right panel.

    * To manually create the segment logic, using segments available on the [Third Party Segments, First Party Segments, Adobe Segments, Custom Segments, and Saved Audiences tabs](audience-settings.md), do the following.

        * To add the first segment, locate the segment in the left panel, and select the check box next to the segment name.

        * To add a segment to an existing segment group:
        
            1. Click the segment group in the right panel.

            1. (Optional) Change the group logic to *Include Any*, *Include All*, or *Exclude All*, as needed.

               *Exclude All* isn't available to the first segment group. For an audience that includes only exclusions, build this audience as *Include Any* and then, within a placement, select that audience from the Excluded Audiences menu.

            1. Locate the new segment in the left panel, and select the check box next to the segment name.
            
               The segment group is automatically updated with the new segment.

        * To add a new segment group:

            1. Click **+ New Group** in the right panel.

            1. (Optional) Change the logic between the previous group and the new group to *And* or *Or*, as needed.

            1. Locate the segments for the new group in the left panel, and select the check boxes next to the segment names.

            1. (Optional) Change the group logic to *Include Any*, *Include All*, or *Exclude All*, as needed.

    * To use segment logic from an existing audience:
    
        1. Copy the segment logic from the existing audience in any of the following ways:
        
            * In the All Audiences view, hold the cursor over the audience row, and then click **...More > Copy to Clipboard**.
            
            * In the settings for the existing audience, at the top of the segment logic panel, click **...More > Copy to Clipboard**.
            
            * In a text editor, manually create the segment logic using alphanumeric segment IDs and [Boolean syntax](audience-segment-logic-syntax.md), and copy it to your clipboard.

        1. Click **paste in an audience rule to begin building**, paste the existing segment logic into the input field, and then click **Apply**.

           >[!NOTE]
           >
           >If the audience already includes any segment logic, pasting in new segment logic overwrites the existing logic.

1. Click **Create**.

>[!MORELIKETHIS]
>
>* [About Audience Management](audience-about.md)
>* [Audience Settings](audience-settings.md)
>* [Syntax for Audience Segment Logic](audience-segment-logic-syntax.md)
>* [Available Third-party Data Providers](audience-third-party-data-providers.md)
>* [Create and Implement a Custom Segment](audience-create-custom-segment.md)
>* [Create and Implement a CCPA Opt-Out-of-Sale Segment](audience-create-ccpa-opt-out-segment.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
