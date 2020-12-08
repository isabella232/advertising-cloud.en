# Collaborative documentation for Advertising Cloud

This is the documentation repository for Adobe Advertising Cloud, including cross-product, DSP, and TV docs. (Later, it will include docs for Creative and Search.)

**Note: This page isn't published in the customer-facing documentation.**

## TOC

+ `TOC.md` at the root of any user guide provides the organization of the topics that are contained in the guide. 
+ Each user guide has a unique `TOC.md`, in which you can order all the pages/topics as necessary.


## User Guide

+ The introduction to the user guide is called `overview.md`
+ Each topic in the user guide has it's own distinct directory.
    + If there is a topic in the guide called *Implementation*, the corresponding directory is `/implementation`
+ All image assets are stored in `/assets` at the root of the user guide.
    + All images in the `/assets` directory will be localized.
    + Any images in the `/no-localize` directory will not be localized (there's a surprise!). This can be used to ensure in loc versions that specific assets aren't reproduced unnecessarily.

## User Guide Level Meta Data

+ Meta data which describes the user guide is stored in the `TOC.md`. This includes:
    + product - name of product/capability.
    + cloud - cloud to which this product belongs.
    + audience - audience or archetype at whom the guide is targeted.
    + user-guide - name of the user guide.

## Page Level Meta Data

+ Meta data required to describe a document is stored as part of each individual page. This includes:
    + title - title of the page
    + description - description of page
    + seo-title - seo alternative title
    + seo-description - alternative title for SEO purposes
    + short-title - (optional field)
    + index - yes / no - will the page be indexed by Adobe's search platform
    + translate - yes / no - will this page be localized
    + beta - is this product in beta?
    + redirect - can be used to create a ref to a new page should that be required
    + doc-type: reference (default) / troubleshooting / developer / tutorial / kb / whitepaper
    
## More Information

For more publishing instructions, style guides, samples and other resources, see:

+ [Contributing author guidelines **specifically for Advertising Cloud**](https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=EfficientFrontier&title=Contributing+Author+Guidelines+for+Advertising+Cloud+Help)
+ [Collaborative authoring for all Adobe writers](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/home.html)

See also:

+ contributing.md For an overview of how to contribute to the documentation.
<!-- * guidelines.md For an overview on what is expected in contributions and how to compose your documentation contributions. -->
+ code-of-conduct.md For an overview of the standards of behavior we expect as you contribute to this documentation project.
