---
title: FAQ About Campaign Management
description: FAQ About Campaign Management
---
# FAQs About Campaign Management

## Latency of Setting Changes

* When you change a placement or package setting, when will the change take effect?

    <!-- This doesn't really answer the question but is vague about the lag time. -->
    
    **[Edit this] XX changes take up to NN hours to take effect.**
    
    If it's the final day of delivery, make changes early in the day so DSP has plenty of time to recalibrate the package based on the changes. For example, if you change from even pacing to frontload pacing, DSP needs to reassess the pacing timeline **[pacing forecast? "pacing line" sounds cryptic]** <!--wording? --> and understand how much it needs to deliver. Don't make that kind of change if you only have one hour left to deliver on the final day of the flight.

## Budget Updates Mid-Flight

* When you make a change to a placement, how long does DSP take to reallocate the **[campaign? package?]** budget? **[1) The answer doesn't actually answer this question; I added a sentence with placeholder below. 2) Define "change":  does this refer only to changes to any of the various placement settings, or does it also include the inclusion/removal of ads/creatives? 3) Will changes to a placement result in changes to only that placement's budget, or might it potentially change the budgets for all other placements within the same package or campaign?]**<!-- see comments -->?

    Budget allocation is based on placement performance, which is evaluated using a 14-day average. Changes to a placement result in changes to the budget allocation only when they cause changes in performance during the 14-day average.

    **[Fill in/edit this] When performance changes occur, DSP can take up to NN hours to reallocate the [campaign or package?] budget among the placements accordingly.**

* How is budget reallocated when a placement is removed from a package and added to another package?

    A placement's entire spend history is attached to the placement and moves with it from package to package.
    
    When you remove a placement from a package, the package no longer has any history of the placement's spend. The daily package budget will become (package budget - removed placement budget) / days remaining in flight. The package budget is then allocated to the placements remaining in the package. **[Verify wording. Also, this talks about a daily package budget, but can we just remove the word "daily?" What if the package budget is for a different interval, like "All time" or "Monthly?"]**<!-- see comments -->
    
    Similarly, if you add the same placement to a different package, DSP considers the placement's spend history when it allocates budget for all placements in the new package. **[Verify behavior and wording]**<!-- see comments -->

* How does a package behave differently on the last day of a flight?

    On the last day of a flight, the day is shortened from 24 hours to 23 hours so that the package budget isn't exceeded. Also, the package's pacing fill strategy automatically changes to "Frontload," even if it's set to "even." This means 65% of the daily budget should deliver by 11:30 a.m. EST.
