---
title:
description:
seo-title:
seo-description:
---

# Image Creatives

## Add Image Creatives

Image files must be in GIF, JPEG, JPG, or PNG format and can be up to 2 MB. See the supported creative sizes.

1. In the main menu, click Creative Library.
1. Click Add Creatives, and then click Image.
1. Specify the images:
   * For local image assets, do either of the following:
     * Drag and drop files on your computer or network into the box.
     * Click [!UICONTROL Browse] from computer to locate the file on your computer or network.
   * For Adobe Creative Cloud image assets, do the following:
     1. Click [!UICONTROL CC Asset Library], and then click [!UICONTROL Launch Asset Selector].
     1. (If you're not already logged in to Creative Cloud from the same browser) Log in to Creative Cloud using your Adobe ID for Creative Cloud, which is different than your login for Creative.
     1. (The first time you log in from Creative) In the prompt to allow Advertising Cloud Creative to access your files, click [!UICONTROL Allow Access].
     1. Select the images:
        * Below each image you want to upload, click + to select it.
          The select icon is shown for each image.
        * Click [!UICONTROL Open].

   * For Adobe Experience Manager image assets, do the following:

     >[!NOTE]
     >
     >Before you can upload assets, you must configure Adobe Advertising Cloud Creative to access Adobe Experience Manager image assets.

     * Click [!UICONTROL AEM Asset Library].
       >[!NOTE]
       >
       >* (If you're not already logged in to Experience Manager from the same browser) Log in to Experience Manager using your Adobe ID for Experience Manager, which is different than your login for Creative.
       >* (The first time you use Experience Manager) In the prompt to allow Advertising Cloud Creative to access your files, click [!UICONTROL Yes, I authorize this request].
       >* When the Experience Manager instance calls back to the Creative server, Creative will retrieve the `access_token` and `refresh_token`. Creative will use the refresh_token to download asset images during future contact with Experience Manager.

     * Select the images:
       * Expand each asset folder until you locate the images you want to upload.
       * Next to each image you want to upload, click the select icon ( ).
       * Click [!UICONTROL Select].
1. Specify the image creative settings.
   By default, all of the creatives you just uploaded are selected, and any settings you specify will apply to all selected creatives. To enter settings for specific creatives, deselect each inapplicable creative.
1. Click [!UICONTROL Save].
