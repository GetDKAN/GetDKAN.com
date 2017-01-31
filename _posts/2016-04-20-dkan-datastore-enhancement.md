---
layout: post
title: "DKAN Datastore Enhancement: bigger files, painless import"
author: "Dawn McDougall"
meta: "DKAN, Open data, Open source, OpenSaaS"
---

Read our [full release notes](https://github.com/NuCivic/dkan/releases/tag/7.x-1.12) on our [public GitHub repo](https://github.com/NuCivic/dkan) and learn about other new features in the latest release, including [DKAN Workflow](http://www.nucivic.com/new-feature-alert-dkan-workflow/) and [DKAN Topics](http://www.nucivic.com/dkan-topics-feature-focus-data-and-reflect-citizen-interests/).

Government organizations are (perhaps surprisingly) major sources of big data. Departments track and collect movement and activity of hundreds of thousands of people. That translates into millions of rows of information all contained in a single file. Large files can be a challenge both to manage and make accessible for a wider audience. In open data efforts, large files must be uploaded quickly and effectively supported for government agencies as well as made consumable for citizens.

We wanted to increase the capacity of the DKAN Datastore to meet both these needs.

In the latest release, we improved the DKAN Datastore import and support of large files to generate better data previews and a more robust API. DKAN defaults to use the Drupal file importer used in previous versions of DKAN, but an additional fast import option can be enabled and configured on DKAN 7.12. For more technical details, read our full release notes on our public GitHub repo. You can also learn about other new features in this release, including DKAN Workflow and DKAN Topics.

## Highlights

- **For DKAN implementors**: With **Large File Support** the **DKAN Datastore** can hold large CSV file sizes (up to a few GB) and the **Fast Import** option greatly reduces import time for large files.
- **For DKAN site visitors**: It’s easier to import large files into the **DKAN Datastore**, so large files can be explored with **DKAN Data Previews**.
- **For Developers**: Easy import and large files in the **DKAN Datastore** translates into a more robust **DKAN Datastore API**.

### Some basics about the DKAN Datastore

<a href="{{site.baseurl}}/img/uploads/2016/04/datastore-image-01.png"><img class="size-full wp-image-3756 aligncenter" src="{{site.baseurl}}/img/uploads/2016/04/datastore-image-01.png" alt="datastore image 01" width="754" height="67"></a>

DKAN comes standard with a datastore to house tabular data formatted as CSV files. That is, the datastore can support files with contents that appear as a table (rows and columns). When adding resources to DKAN there are two options:

1. **Simply upload the file and nothing else**. The resource will appear on the site and be available to site visitors for download. Certain files (depending on format and size) may be previewed.
2. **Upload the file and import the file into the datastore**. For all practical purposes, the resource appears the same to site visitors.

So if the resource is practically the same either way, why import into the datastore? The real difference happens behind the scenes.

<a href="{{site.baseurl}}/img/uploads/2016/04/datastore-02.png"><img class="alignnone wp-image-3757" src="{{site.baseurl}}/img/uploads/2016/04/datastore-02.png" alt="datastore 02" width="650" height="501"></a>

A simple upload makes the data available but not necessarily accessible.

In the case of large files, citizens can’t explore resources visually unless the file is first imported into the Datastore. With small files, you might not notice much of a difference. But what if you have a file that contains hundreds of thousands (or even millions) of rows? Files of this size uploaded (but not imported) don’t appear in the previews commonly used to show a snapshot of resources on DKAN.

### Some basics about DKAN Data Previews

Previews connect citizens to data by allowing them to see a snapshot of the data before (or instead of) downloading the entire file. Preview tools give users the option to see a basic visual of a resource as a grid, chart, or map.

<a href="{{site.baseurl}}/img/uploads/2016/04/datastore-image-03.jpg"><img class="alignnone size-full wp-image-3758" src="{{site.baseurl}}/img/uploads/2016/04/datastore-image-03.jpg" alt="datastore image 03" width="1740" height="636"></a>

Data Previews let citizens take a quick look at the data contained in a resource and easily share data insights with their social and professional networks. Adding Large File Support and Fast Import to the DKAN Datastore makes it painless to import large resources, which means better Data Previews regardless of the file size. And that means a better citizen experience.

The Large File Support enhancement for the DKAN Datastore also translates into a better API.

Resources are inaccessible to programmers when they are only uploaded and not imported. Files imported into the DKAN Datastore are included as part of the DKAN Datastore API that provides an access point for technical users to consume the data programmatically. With Large File Support, the DKAN Datastore can store more resources and their data which translates into a better API.

### Some basics about the DKAN Datastore API

DKAN comes standard with two APIs including the DKAN Datastore API. APIs are created for technical users and are critical to the usability of data. APIs are the key that enable digital tools and computer programs to “talk” to one another. APIs act like a door to let programs get in behind the scenes but only for certain areas. So technologists can get access to a “room” but not the entire house (ie an entire website).

<a href="{{site.baseurl}}/img/uploads/2016/04/datastore-image-04.png"><img class="alignnone size-full wp-image-3759" src="{{site.baseurl}}/img/uploads/2016/04/datastore-image-04.png" alt="datastore image 04" width="900" height="144"></a>

<a href="{{site.baseurl}}/img/uploads/2016/04/datastore-image-05.png"><img class="alignnone size-full wp-image-3760" src="{{site.baseurl}}/img/uploads/2016/04/datastore-image-05.png" alt="datastore image 05" width="1388" height="118"></a>

As you might imagine, the Datastore API has all the information about the files that have been imported into the datastore from a high-level (title, data, etc) down to very specific info (a single row or column). Including data in the DKAN Datastore API greatly increases the discoverability of the information as well as its usability and accessibility. Without the DKAN Datastore API, data could not be searched with such precision.

Resources imported to the DKAN Datastore are included in the Datastore API and usable for programmers. Resources that are simply uploaded are not.

With the DKAN Datastore API, technical users can write programs to interact with the information held within the API. This means that the data in the DKAN Datastore can be accurately and efficiently queried (searched) and the data then used in other contexts and applications. This feature is another way to show how open data can be used to provide a tangible return for citizens.

Tl;dr

- Government agencies need a way to manage large files quickly and effectively. In DKAN 7.12, **Large File Support** and **Fast Import** can import and store large files within minutes.
- Citizens need to understand large amounts of information without extensive technical knowledge. **Large File Support** and **DKAN Data Previews** make it possible.
- Technical citizens need to have access to large quantities of data programmatically. **Large File Support** and the **DKAN Datastore API** create the access point.
- The **DKAN Datastore** is a powerful support mechanism for **Data Previews** and the **Datastore API**–core elements in the usability of data and the user experience on a DKAN site.
- **Large File Support** broadens the **Datastore API** and creates **Data Previews** for files of almost any size.
- **Fast Import** makes it possible to import large files into the DKAN Datastore in a matter of minutes.

The Datastore only works for files uploaded and then imported in. Here’s when to use the Datastore:

- The file is formatted as a CSV.
- File contents include thousands (to millions) of lines and the size is up to a few gigabytes.
- To include the file as part of the **DKAN Datastore API**.

If all else fails just remember–when in doubt, import!

Read our [full release notes](https://github.com/NuCivic/dkan/releases/tag/7.x-1.12) on our [public GitHub repo](https://github.com/NuCivic/dkan) and learn about other new features in the latest release, including DKAN Workflow and DKAN Topics.

Are you a developer and want to use and/or contribute to DKAN? DKAN is open source and accepts contributions–check out our [public GitHub](https://github.com/NuCivic/dkan).

Want DKAN’s enterprise solution? [Test drive DKAN](http://demo.getdkan.com/) and [contact our team](mailto:contact@nucivic.com) for more information.
