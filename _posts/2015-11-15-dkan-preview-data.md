---
layout: post
title: "Now you can preview data with external tools on DKAN"
author: "Federica Pelzel"
meta: "DKAN, DKAN Launch, Drupal open data, Featured DKAN, Open data, Open source"
---
With the release of [DKAN 7.x-1.10](https://github.com/NuCivic/dkan/releases) we’re shipping a new feature called “**External Previews**“. This feature allows users to preview a wider range of data formats with specialized external tools, integrated seamlessly with DKAN. You may have seen this feature on [Data.gov](https://www.data.gov/meta/open-apps/) before, and now you can get it for free, out of the box with DKAN.

We believe in building a great product, that becomes better as it empowers and integrates with specialized tools that fulfill specific needs, adding value to your data. In this first iteration we’re including External Previews that use CartoDB and ArcGIS, extending DKAN’s preview format compatibility to include ***rest, esri rest, arcgis, excel, openxml, kml,*** *and* ***geojson***.

<img class="aligncenter wp-image-3375 size-full" src="{{site.baseurl}}/img/uploads/2015/11/Screen-Recording-2015-11-17-at-03.28-PM.gif" alt="feature gif" width="838" height="509">

## CartoDB

CartoDB is an easy to use mapping tool that allows you to create, customize, and analyze geographic data in an intuitive way. For more information on CartoDB and it’s capabilities check out [cartodb.com](https://cartodb.com/).

To open a resource with CartoDB, all you need to do is identify the option, click “**CartoDB Preview**” and follow the instructions. If you don’t have a CartoDB account yet, you’ll be asked to create one. Account pricing ranges from free to enterprise, more info [here](https://cartodb.com/pricing/).

<img class="aligncenter wp-image-3385 size-full" src="{{site.baseurl}}/img/uploads/2015/11/Screen-Recording-2015-11-18-at-12.31-PM.gif" alt="Screen Recording 2015-11-18 at 12.31 PM" width="1439" height="691">

Once your data in loaded in CartoDB you can use it to create your own maps, which you can save and publish as desired. If you’re a DKAN or Granicus Data authenticated user, you can later embed any maps you create in Dashboards or Data Stories.

To learn more of what you can do with CartoDB and how visit their [Map Academy](http://academy.cartodb.com/).

## ArcGIS

ArcGIS is ESRI’s tool for analyzing and mapping geographic data. Resources linking to ArcGIS will usually show fully built maps that have already been configured by the uploader. You can edit and tweak these maps and save to your account. To learn more about ArcGIS and its features visit [arcgis.com](http://www.arcgis.com/home/index.html).

As with other external previews, ArcGIS will require you to create an account when trying to open a resource.

<img class="aligncenter size-full wp-image-3399" src="{{site.baseurl}}/img/uploads/2015/11/Screen-Recording-2015-11-18-at-02.50-PM.gif" alt="Screen Recording 2015-11-18 at 02.50 PM" width="1439" height="632">

## Configuration

Make sure you’re on DKAN version [7.x-1.10](https://github.com/NuCivic/dkan/releases) or later. Log in, and from the “DKAN” menu at the top click on “DKAN Dataset Previews”.

Once you’re on the configuration page you’ll see a list of formats and suggested external previews that can be enabled for each one. Check all the ones you want to enable and click on “Save Configuration”.

<img class="aligncenter wp-image-3389 size-full" src="{{site.baseurl}}/img/uploads/2015/11/Screen-Recording-2015-11-18-at-12.57-PM.gif" alt="Screen Recording 2015-11-18 at 12.57 PM" width="1439" height="691">

When you’re uploading/creating resources, make sure you specify their format so the External Previews become available.

## Get it today

You don’t need to be a developer to install and set up your own DKAN instance. Get started for free with DKAN on Pantheon [here](https://dashboard.getpantheon.com/products/dkan/spinup), and follow the instructions.

If you already have a working DKAN instance please update to the latest release and follow the instructions above.

If you’re a [Granicus Data](http://www.nucivic.com/data/) customer please contact support and we’ll take care of you.

We plan to continue working on integrating better and with more companies that deliver a richer data experience for you and your users. If you have any feedback or ideas please reach out to us or leave a comment below.
