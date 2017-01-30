---
layout: post
title: "New Feature Alert: DKAN Workflow"
author: "Dawn McDougall"
---

Read our [full release notes](https://github.com/NuCivic/dkan/releases/tag/7.x-1.12) on our [public GitHub repo](https://github.com/NuCivic/dkan) and learn about other new features in the latest release, including [DKAN Topics](http://www.nucivic.com/dkan-topics-feature-focus-data-and-reflect-citizen-interests/) and [DKAN Datastore enhancements](http://www.nucivic.com/dkan-datastore-enhancement-bigger-files-painless-import/).

In the latest version of DKAN, we’ve added a feature called Workflow. Workflow makes it possible to moderate content with a large team of contributors managing data on a DKAN site. This ensures that many data providers are able to contribute data without needing to compromise data quality. Don’t worry, you won’t need a red pen.

<img src="https://farm3.static.flickr.com/2090/2349630643_712c43496b.jpg" alt="paper edited with red ink" width="633" height="421">

In a previous post, we announced a [DKAN Roles and Permissions module](http://www.nucivic.com/dkan-roles-and-permissions-just-got-easier-in-the-latest-release/) that includes the default “core” user roles provided out of the box. We believe that this will help streamline the process of standing up a data portal and relieve possible confusion when deciding on which roles to provide on a site and which permissions will be associated with these roles.

Though these default roles come pre-loaded, the option to customize roles and permissions still exists. This is because although there may be some common needs met by the six built-in roles, every site has specific needs that will require tweaking some permissions associated with roles or creating new combinations all together.

In addition to the core roles, the latest release of DKAN includes a set of modules that together we call **DKAN Workflow**. It opens additional functions to manage an editorial review process. Though distinct from core roles and permissions, Workflow roles give an additional layer of capability to DKAN users. This post will go into more detail about workflows, the Workbench module, and roles that are specific to the process.

**Note:** This module is not automatically enabled with DKAN, so administrators will need to determine whether the Workflow features are necessary for their needs. Workflow is a powerful feature, but it can overcomplicate working with the site if the situation doesn’t call for all of the capabilities it adds.

## Workflows and the editorial review process

Data portals can house thousands of files in the form of **resources** organized into **datasets**, and these datasets and resources may originate from a variety of departments and organization. While there are usually only one or two site managers  – Site Manager is a core role – maintaining the entire site, resources can be added by dozens of different users from various sources. This empowers agencies to add their data as it becomes available and allows for updating the data portal to be a sustainable endeavor.

On the other hand, broad contributions add a complicating factor for Site Managers. Contributors from different groups can add data to the portal, but these users may be unfamiliar with open data standards and less knowledgeable about handling data in general.

Moreover, there are users for whom you may want to check over their work before it’s submitted. For example, if a new intern in a local City Planning department has been tasked with uploading new datasets to the city’s open data portal, the intern’s manager may want to review his or her work to ensure its quality and accuracy before it is uploaded live to the site. How can the manager oversee their intern’s work quickly and easily? Enter DKAN Workflow.

## DKAN Workflow

The DKAN Workflow module creates a moderation queue so that content is published only after a designated supervisor has reviewed and approved it. Contributors can still add content to the data catalogue, but it is up to a supervisor to act as the gatekeeper in making the content public on the live site.

<a href="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-4.13.50-PM.png"><img src="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-4.13.50-PM.png" alt="DKAN moderation queue" width="950" height="276"></a>

### Here’s how it works

Content exists in three states:

1. “Draft”  – A saved work in progress.
2. “Needs Review” – The author feels the content is ready to go on public on the live site, and would like the supervisor to review it.
3. “Published” – The content is public and visible on the live site.

There are two key components of the DKAN Workflow module: Workflow-specific roles and the Workbench module with some DKAN-specific customizations. [Workbench](https://www.drupal.org/project/workbench) is a widely-used Drupal module with its [own extensive documentation](https://www.drupal.org/node/1171018).

In brief, Workbench provides Drupal with more robust content management via a system of “states” (a piece of content could be in either a “draft” state, a “needs review” state, or a state with any other arbitrary name before ultimately being published) and “transitions” (which define in which order content can move from state to state, and who has permissions to do so). As content is drafted, it goes through an editorial workflow managed by trusted roles.

<a href="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-5.10.26-PM.png"><img src="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-5.10.26-PM.png" alt="DKAN Workbench Feature" width="954" height="483"></a>

### Workflow Specific Roles

Each user will have a role (or multiple roles, given their status within the organization) and have certain permissions for moving content through the workflow. These roles allow users to interact differently with Workbench, but they do not negate the need for [core roles](http://www.nucivic.com/dkan-roles-and-permissions-just-got-easier-in-the-latest-release/).  This means that every user must be assigned a core role granting a certain level of access to the site, independent of the DKAN Workflow module and the user’s role within that module.

Core roles/permissions and Workflow roles/permissions serve different purposes but work in complement. Each set of roles has different permissions that enable the user to interact with certain functions on DKAN. As Workflow roles are assigned, DKAN will automatically select the core role equivalent so that there are no gaps in a user’s permissions.

<a href="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-5.34.15-PM.png"><img src="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-5.34.15-PM.png" alt="Workflow and Core Roles" width="451" height="270"></a>

Here’s how it works – there are three roles with Workflow-specific permissions:

1. **Workflow Contributor**
2. **Workflow Moderator**
3. **Workflow Supervisor**

#### Workflow Contributor

The **Workflow Contributor** role has the lowest level of permissions while still providing access to Workbench. These users are generally adding to the data catalogue, but their content needs approval before it is published and made live. In the aforementioned scenario regarding a college intern uploading resources to a city open data site, the intern would have this role. As a Workflow Contributor, they can save content as a “Draft” or move it to “Needs Review,” but they do not have the power to publish content live.

**Note:** Workflow Contributors will be assigned the core role of “**Content Creator**.”

#### Workflow Moderator

The **Workflow Moderator** role has the most crucial job of the three Workflow-specific roles. The Workflow Moderator is tasked with reviewing all content that has been added by Workflow Contributors for a single group and moving it through the publishing pipeline. In the case of the college intern whose content needs to be reviewed before it is published, the Workflow Moderator would likely be his or her manager.

This role reviews and publishes content – including what they have created themselves – for their group, rather than the entire site. On a hypothetical open data site, the Workflow Moderator for the City Planning department would not be able to moderate the workflow of content for the Public Health department – only data and content associated with the group City Planning.

Moderators can also “unpublish” content, leaving it in a “Needs Review” or “Draft” state and removing it from public view, or delete content altogether.

**Note:** Workflow Moderators will be assigned the core role of “**Editor**.”

How can Workflow Moderators manage content effectively? Workflow Moderators should ensure that data uploaded to the site does not have any sensitive or private information included within it. They should also check whether the file format is listed correctly, that the resource follows open data best practices, and that is associated with the correct licenses. Lastly, the Workflow Moderator should look over the dataset or resource’s metadata and ensure that it is accurate and as thorough as possible.

#### Workflow Supervisor

The Workflow Supervisor role has the highest-level permissions within Workflow because users with this role are not restricted to group to which they belong. Unlike a Moderator, a Supervisor belonging to the group City Planning is able to modify content within the group Public Health.

Supervisors can access content from all groups and moderate content as needed. However, the primary focus of the supervisor is administering Workbench for the entire site. In general, this is an administrative role rather than a practical one. Supervisors catch any issues that could otherwise fall through the cracks, especially in the case of content that isn’t associated with a specific group.

**Note:** Workflow Supervisors will be assigned the core role of “**Site Managers**.”

<table style="height: 133px;" width="747">
<tbody>
<tr>
<td><b>Core Role</b></td>
<td><span style="font-weight: 400;">Content Creator</span></td>
<td><span style="font-weight: 400;">Editor</span></td>
<td><span style="font-weight: 400;">Site Manager</span></td>
</tr>
<tr>
<td><b>Workflow Role</b></td>
<td><span style="font-weight: 400;">Workflow Contributor</span></td>
<td><span style="font-weight: 400;">Workflow Moderator</span></td>
<td><span style="font-weight: 400;">Workflow Supervisor</span></td>
</tr>
</tbody>
</table>

### How do the different workflow-specific roles use Workbench?

<a href="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-3.48.21-PM.png"><img src="{{site.baseurl}}/img/uploads/2016/03/Screen-Shot-2016-03-28-at-3.48.21-PM.png" alt="DKAN Workbench Tabs" width="897" height="197"></a>

Workbench stores unpublished content in the “Draft” and “Needs Review” states, while the above roles give certain users the ability to moderate content through the editorial workflow. Users can view the state of the content as well as its age.

DKAN Workflow is unique in that it organizes content into five different tabs, grouped by its moderation status: My Content, My drafts, Needs Review, Stale Drafts, and Stale Reviews.

The “Stale Drafts” and “Stale Reviews” tabs contain content that has gone untouched for too long – hence the term “stale.” The default time limit in DKAN is 72 hours before drafts become stale.

For Workflow Moderators who are reviewing a steady stream of content, it’s helpful to know how many pieces of content need to be moderated. In the picture above, note that each tab has a bubble with a number located in the top right corner. This number reflects the total pieces of content within that tab.

For example, as a Workflow Moderator I may have two drafts and 10 pieces of content waiting for me in “Needs Review”. Two of my drafts may have gone stale and would also appear in my “Stale Drafts” tab. Three of my reviews may also be stale and would appear both in my “Needs Review” tab as well as the “Stale Reviews” tab. The quantities of content within each category will appear as a count at the top of each tab.

As a Workflow Contributor, I may have active drafts and stale drafts but will not be able to view any content within “Stale Reviews”. This is because users with certain roles will only see the content that the role’s permissions allow.

The following table provides details on the permissions associated with Workflow roles:

<table>
<tbody>
<tr>
<td><b>Tab</b></td>
<td><b>Role (Who can view the tab?)</b></td>
<td><b>What the tab displays</b></td>
</tr>
<tr>
<td><span style="font-weight: 400;">My Content</span></td>
<td><span style="font-weight: 400;">All Workflow Roles</span></td>
<td><span style="font-weight: 400;">All of the content that a user has authored, in any publishing stage</span></td>
</tr>
<tr>
<td><span style="font-weight: 400;">My Drafts</span></td>
<td><span style="font-weight: 400;">All Workflow Roles</span></td>
<td><span style="font-weight: 400;">All of the user’s own drafts</span></td>
</tr>
<tr>
<td><span style="font-weight: 400;">Needs Review</span></td>
<td><span style="font-weight: 400;">All Workflow Roles</span></td>
<td><span style="font-weight: 400;">For </span><strong>Workflow Contributors</strong><span style="font-weight: 400;">, this will be content that they have moved to the “Needs Review” state.</span><p></p>
<p><strong>Workflow Moderators</strong><span style="font-weight: 400;"> see “Needs Review” content for their specific group.</span><span style="font-weight: 400;"><br>
</span><span style="font-weight: 400;"><br>
</span><strong>Workflow Supervisors</strong><span style="font-weight: 400;"> see “Needs Review” content for the entire site. &nbsp;</span></p></td>
</tr>
<tr>
<td><span style="font-weight: 400;">Stale Drafts</span></td>
<td><span style="font-weight: 400;">Workflow Moderators and Supervisors</span></td>
<td><span style="font-weight: 400;">All drafts that are more than 72 hours old.</span></td>
</tr>
<tr>
<td><span style="font-weight: 400;">Stale Reviews</span></td>
<td><span style="font-weight: 400;">Workflow Moderators and Supervisors</span></td>
<td><span style="font-weight: 400;">All “Needs Review” content that has been in that state for more than 72 hours.</span></td>
</tr>
</tbody>
</table>

## Tl;dr:

- The DKAN Workflow module organizes content in various states of an editorial workflow, using the Workbench module as a base.
- Workbench on DKAN creates a system of “states” (“Draft,” “Needs Review,” and more) and “transitions” (which define the order that content can move from state to state, and who has permissions to move the content between states). These states are part of moderating content, which is essential for handling lots of content generated and edited by several users.
- As part of the new module, Workflow-specific roles and permissions determine how a user interacts with Workbench states. There are three roles for DKAN Workflow: Workflow Contributor, Workflow Moderator, and Workflow Supervisor.
- Core roles/permissions and Workflow roles/permissions serve different purposes but work in complement. Each set of roles is simply given different permissions that enable a user to interact with certain functions on DKAN. The level of access on the Workbench reflects a user’s access to the rest of the site. When assigning roles to users, selecting a Workflow role automatically also associates the user with a core role.

<table>
<tbody>
<tr>
<td><b>Core Role</b></td>
<td><span style="font-weight: 400;">Content Creator</span></td>
<td><span style="font-weight: 400;">Editor</span></td>
<td><span style="font-weight: 400;">Site Manager</span></td>
</tr>
<tr>
<td><b>Workflow Role</b></td>
<td><span style="font-weight: 400;">Workflow Contributor</span></td>
<td><span style="font-weight: 400;">Workflow Moderator</span></td>
<td><span style="font-weight: 400;">Workflow Supervisor</span></td>
</tr>
</tbody>
</table>

- Workflow Contributors are tasked with adding content, and it is the moderator of a group who is focused on the quality of the content itself for a single group. Supervisors oversee moderation for all groups to catch anything that might slip through the cracks, but are not involved in daily moderation.
- Users have additional tabs on Workbench including “My Content” which shows users all of their content in one place. The tabs “Stale Drafts” and “Stale Reviews” list content that has exceeded a designated time-limit.
- The Workbench is customized to show the content count in a certain state. For example, how many drafts or pieces in review a user has. Moderators can see how many “stale” items are in still waiting for review.
- As a default, content becomes “stale” if it exceeds 72 hours without changes. This can be customized to better suit individualized contexts.

<img src="https://upload.wikimedia.org/wikipedia/commons/9/9b/Social_Network_Analysis_Visualization.png" alt="" width="711" height="530">

Dealing with dozens – sometimes hundreds – of users naturally adds complexity to managing a DKAN data portal. How can data owners contribute their resources without needing to overcome a steep learning curve or inadvertently doing damage to the site? How can Site Managers feel confident that content meets certain standards without tediously poring over the data themselves?

DKAN Workflow answers these questions by adding a mechanism for moderating content as part of an editorial workflow powered by Workbench. Lower-access users can still add content, and Moderators can check its quality before it is made public. Workbench is also helpful in organizing content and making the management process more efficient.

Though handling a large number of users with a number of different roles and permissions can seem daunting at first, DKAN Workflow is possibly one of the most powerful features for Site Managers. Both a way to empower others to engage with open data while still maintaining control over the quality of content, DKAN Workflow offers a balanced solution.

Read our [full release notes](https://github.com/NuCivic/dkan/releases/tag/7.x-1.12) on our [public GitHub repo](https://github.com/NuCivic/dkan) and learn about other new features in the latest release, including DKAN Topics and DKAN Datastore enhancements.

Are you a developer and want to use and/or contribute to DKAN? DKAN is open source and accepts contributions–check out our [public GitHub](https://github.com/NuCivic/dkan).

Want DKAN’s enterprise solution? [Test drive DKAN](http://demo.getdkan.com/) and c[ontact our team](mailto:contact@nucivic.com) for more information.
