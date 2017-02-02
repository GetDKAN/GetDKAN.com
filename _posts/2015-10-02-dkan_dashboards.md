---
layout: post
title: "DKAN 1.9 Features “Drag and Drop” Data Dashboards"
author: "Aaron Couch"
meta: "DKAN Launch, Featured DKAN"
---

NuCivic is proud to announce the release of DKAN version 1.9. Developers can grab the latest code on [Github]. Open Data enthusiasts can spin up a version for themselves for free at our hosting partners [Acquia] and [Pantheon].

Drag and Drop Layouts
---------------------

DKAN now supports “drag-and-drop” layout for all pages on the site. This allows non-developers to updating existing pages by adding custom content, widgets or other data visualization tools:<img src="http://www.nucivic.com/wp-content/uploads/2015/10/image03.gif" alt="Drag and drop layout" class="alignnone wp-image-3327" width="408" height="360" /> or change the layout of existing pages: <img src="http://www.nucivic.com/wp-content/uploads/2015/10/image01.gif" alt="layout options" class="alignnone wp-image-3328" width="408" height="360" /> This functionality is provided by Drupal’s [Panels] module which has become the most popular layout solution in Drupal. Administrators using DKAN can now click “Customize this Page” to expose the drag-and-drop interface: <img src="http://www.nucivic.com/wp-content/uploads/2015/10/image04-1024x651.png" alt="image04" class="alignnone wp-image-3329" width="705" height="448" /> Administrators have over a dozen layouts to choose from: <img src="http://www.nucivic.com/wp-content/uploads/2015/10/image05-1024x651.png" alt="image05" class="alignnone wp-image-3330" width="703" height="447" /> Layouts are fully responsive for desktop and mobile users. See [our documentation] for full details.

Data Stories and Data Dashboards
--------------------------------

The 1.9 release adds the ability to create data-driven dashboards. We’ve made this easy with a several new tools:

-   drag-and-drop layouts for data dashboards
-   native visualization tools
-   easy integrations with outside visualization tools

Our drag-and-drop layouts are described above. We also have the option of adding map data, slideshows, videos, and other storytelling tools to our dashboard tool.

Native Visualization Tools
--------------------------

DKAN 1.9 includes the ability to create graphs, charts, and maps with your portal’s data using our native visualization tools. These tools include a charts and graphs wizard that makes it easy to dig into your catalog’s data and exhibit the latests graphs, trends, and available resources. The wizard takes users step by step through selecting, querying, and visualizing data: 

[<img src="http://www.nucivic.com/wp-content/uploads/2015/10/image06.png" alt="image06" class="alignnone wp-image-3331" width="710" height="393" />] We’ve also added a choropleth mapping tool: [<img src="http://www.nucivic.com/wp-content/uploads/2015/10/image02-1024x757.png" alt="image02" class="alignnone wp-image-3332" width="668" height="494" />]

Integrating 3rd Party Visualization Tools
-----------------------------------------

With DKAN 1.9 it’s easy to create data dashboards with graphics, maps, and images created with third-party tools as well. External visualizations can be added directly into dashboards and data stories with a few clicks, and then placed in the desired region on a data dashboard.

Many Other Feature Enhancements, Bug Fixes, and More
----------------------------------------------------

DKAN 1.9 was a big release for us. Some other notable features include an integration with [Font Your Face], which along with our [Colorizer] integration and drag and drop interface described above, lets non-technical users control much of the layout and look of the site. See our full [release notes] for more details.

  [<img src="http://www.nucivic.com/wp-content/uploads/2015/10/image06.png" alt="image06" class="alignnone wp-image-3331" width="710" height="393" />]: http://www.nucivic.com/wp-content/uploads/2015/10/image06.png
  [<img src="http://www.nucivic.com/wp-content/uploads/2015/10/image02-1024x757.png" alt="image02" class="alignnone wp-image-3332" width="668" height="494" />]: http://www.nucivic.com/wp-content/uploads/2015/10/image02.png
  [Github]. Open Data enthusiasts can spin up a version for themselves for free at our hosting partners [Acquia] and [Pantheon]
  
  
  [Github]: https://github.com/nucivic/dkan
  [Acquia]: https://insight.acquia.com/free?distro=dkantestdrive
  [Pantheon]: https://dashboard.getpantheon.com/products/dkan/spinup
  [Panels]: https://www.drupal.org/project/panels
  [our documentation]: http://docs.getdkan.com/dkan-documentation/dkan-users-guide/customize-dkan-pages-layouts-and-components-using-panels
  [Font Your Face]: https://www.drupal.org/project/fontyourface
  [Colorizer]: http://docs.getdkan.com/dkan-documentation/dkan-users/custom-appearance#Color_scheme
  [release notes]: https://github.com/NuCivic/dkan/releases/tag/7.x-1.9
