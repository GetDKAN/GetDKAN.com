---
layout: post
title: "DKAN roles and permissions just got easier in the latest release"
author: "Dawn McDougall"
meta: "DKAN Launch, Featured DKAN"
---

Your website is a great resource for your stakeholders to see the hard work of your organization as well as access important, relevant information. Site visitors should be able to easily navigate the site to find what they are looking for as well as learn about your efforts. The balance between providing thorough information while promoting the most timely and pertinent is an ongoing consideration in managing web content. It takes a team of people working together by playing individual roles that contribute to a larger effort to have a successful site.

<a href="{{site.baseurl}}/img/uploads/2016/01/Screen-Shot-2015-12-15-at-12.11.39-PM.png"><img class="wp-image-3421 alignleft" src="{{site.baseurl}}/img/uploads/2016/01/Screen-Shot-2015-12-15-at-12.11.39-PM.png" alt="DKAN Homescreen" width="498" height="365"></a>

On a website, roles categorize types of users and the associated permissions determine what that user type is allowed to do and see behind the scenes.
It’s the **site administrator** who sets up a site initially. This role generally falls to a highly technical user, and site administrators have every permission possible. But this person won’t necessarily be involved in the daily management of a website. It’s the **site manager** who works hands-on with keeping the site up and running, including bringing in new people on the team.

Many different people with different backgrounds and levels of knowledge working on the same website…it’s no great mystery why roles and permissions are necessary, but it’s also easy for these to quickly get out of control. Previous versions of DKAN had only very basic roles and left the site administrator to define and customize roles and permissions as a starting point.

While this was great for making data portals individualized for specific organizations, we realized there was a growing need for consistent, standardized roles and permissions for DKAN as a product. The latest version comes with a more intuitive set of user roles.

## Core DKAN roles and permissions

Core roles are associated with permissions and those permissions represent functions the users can perform across the site. These permissions are user-level, meaning the role is set in the user’s specific record. There are 6 core roles in the DKAN Permissions module that come out-of-the-box.

1. **Anonymous User**
2. **Authenticated User**
3. **Content Creator**
4. **Editor**
5. **Site Manager**
6. **Administrator**

Below is a detailed table of roles and the permissions included in the new DKAN Permissions module to help show what different user types are able to do on the site and help site managers decide who should have what role. A few of these roles won’t affect the day-to-day of managing the website or the content. Click on the image to see the table in detail on our [documentation site](http://docs.getdkan.com/dkan-documentation/dkan-users/dkan-user-management).

Naturally users will need more than one role to fulfill the full scope of their job. There will also be cases where you need users to have different permissions in the context of a particular group (for instance, to be able to modify content belonging to their agency but not other agencies on the same website). Keep reading after the table to find out more about group permissions.

A note about the new roles: If you are already operating on an older version of DKAN, updating won’t automatically enable this module or migrate your users over to these new roles. We recommend disabling the old “DKAN Sitewide Roles and Permissions” module and enabling the new “DKAN Permissions” module, but be aware that you will probably need to review all of your site’s users to make sure they have the appropriate role going forward.

## Core DKAN Roles and Permissions

<table>
<tbody>
<tr>
<td><b>Role</b><br>
<b>(User Type)</b></td>
<td><b>Description</b></td>
<td><b>Permissions </b><br>
<b>(What can I do?)</b></td>
<td><b>Description</b></td>
</tr>
<tr>
<td>Anonymous User:<br>
<span style="font-weight: normal; font-size: 12px;">General site visitors that are not logged in. </span></td>
<td><span style="font-weight: normal; font-size: 12px;">This user type has no profile information, hence it’s anonymous.</span></td>
<td>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">View and search content on public website. </span></li>
</ul>
<p>&nbsp;</p></td>
<td><span style="font-weight: normal; font-size: 12px;">DKAN recognizes this user type to let it see and search content, but doesn’t let the user add comments. </span></td>
</tr>
<tr>
<td>Authenticated User:<br>
<span style="font-weight: normal; font-size: 12px;">These users are logged on and have profile information that can be verified (and authenticated).</span></td>
<td><span style="font-weight: normal; font-size: 12px;">This type has the lowest level of permissions; all users with login credentials have this role. This user type is a general site visitor but he or she has created an account. </span></td>
<td>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Have a profile and add/edit that profile. </span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Can leave comments on the data catalogue.</span></li>
</ul>
</td>
<td><span style="font-weight: normal; font-size: 12px;">DKAN can verify account information with a created profile so that the user is able to take limited actions and manage profile details. </span></td>
</tr>
<tr>
<td>Content Creator:<br>
<span style="font-weight: normal; font-size: 12px;">Content Creators are focused simply on adding resources to the data catalogue under direction of a supervisor. </span></td>
<td><span style="font-weight: normal; font-size: 12px;">At this level, the role must be assigned by a higher role; this role has access to the production side of the site. This will be someone working in your organization who helps by adding to the data catalogue but doesn’t need to worry about the whole site.</span></td>
<td>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Create most content types and edit own content. </span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">View own unpublished content and revision history of all published content. </span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Add and view files to site library.</span></li>
</ul>
</td>
<td><span style="font-weight: normal; font-size: 12px;">This level of access takes users into the production side of the site, but gives little freedom to move outside of creating and adding certain content types. Limiting this role is critical for avoiding inadvertent damage to site content. </span></td>
</tr>
<tr>
<td>Editor:<br>
<span style="font-weight: normal; font-size: 12px;">This will typically be a person handling the content on a frequent basis. Someone in your organization with expertise on the subject-matter that is expansive as well as in-depth.</span></td>
<td><span style="font-weight: normal; font-size: 12px;">An editor role is similar to a content creator role because the focus is content, however an editor will deal with multiple content authors and have the ability to manage and edit. An editor is responsible for managing content from a strategic perspective. </span></td>
<td>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: 400;">Assign roles to lower-level users.</span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">View, edit, delete most content types and manage versions of content. &nbsp;</span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Access and manage DKAN datastore</span></li>
</ul>
</td>
<td><span style="font-weight: normal; font-size: 12px;">The editor largely handles the quality and timeliness of the content that appears on the site. This role is able to make changes to content and where it appears, but it doesn’t go further into admin functions. </span></td>
</tr>
<tr>
<td>Site Manager:<br>
<span style="font-weight: normal; font-size: 12px;">The highest-level for non-technical users. A site manager is mostly concerned with admin functions of the site. Typically this will fall to someone in a supervisory role. </span></td>
<td><span style="font-weight: normal; font-size: 12px;">The site manager takes a high-level view of the site, its content, and the users on the site. This person maintains the site and assigns roles and permissions to new users but doesn’t deal with the technical backend. </span></td>
<td>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Create, edit, delete all content types created by any user.</span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Change the types of content that lower-access roles can create. </span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Assigns roles to all user levels, but cannot create new roles/perms.</span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Create and manage groups. </span></li>
</ul>
</td>
<td><span style="font-weight: normal; font-size: 12px;">The site manager handles the admin part of the site. This role keeps the production side of the site in good order so that editors and contributors can focus on what site visitors see on the website. This is still largely a non-technical role. </span></td>
</tr>
<tr>
<td>Administrator<br>
<span style="font-weight: normal; font-size: 12px;">The administrator role holds every permission, and it requires high technical competency. This role has the ability to cause serious damage, so it’s generally reserved for a single web professional. </span></td>
<td><span style="font-weight: normal; font-size: 12px;">The administrator handles the overall structure of the website for lower-access roles to plug content into and make changes as needed. Admins hold the highest level of all roles and permissions.</span></td>
<td>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Enable/disable DKAN modules and features.</span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Change the appearance of the site with views and themes.</span></li>
</ul>
<ul>
<li style="font-weight: normal; font-size: 12px;"><span style="font-weight: normal;">Create and edit &nbsp;user roles and permissions. &nbsp;</span></li>
</ul>
</td>
<td><span style="font-weight: normal; font-size: 12px;">Administrators are the middle piece between users using a site daily and the core functions built in the technical backend. Based on an organization’s requirements the administrator can adapt the site to meet daily needs of users.</span></td>
</tr>
</tbody>
</table>

## Group roles and permissions

With large sites there is often a need to have special permissions for a group of users to handle a specific set of content. Think of a large agency or department with sub-departments or programs that produce content. On the one hand these users shouldn’t have the ability to manage or edit content for the entire site or other groups. On the other hand it would be impractical for editors or site managers to handle content for a large number of users. To keep content organized and in the hands of its owners without introducing the risk of inadvertent (and sometimes irreversible) actions, group-level permissions give users the ability to do things they couldn’t necessarily do on the site outside of the group.

Within groups there are different levels of access a user can have, which determines another level of permissions. Any user who belongs to a group falls into one of two categories: **member or administrator**.

As a **member**, a user can create, edit, and delete content within their group. An **administrator** of a group plays a similar role to that of an “editor” but rather than for the entire site it is for their particular group. Conversely, *editors outside of a group are not able to manage content published within a group*. Administrators of groups are able to add and remove group members, manage permissions for group members, and manage (create/edit/delete) all content within the group. It’s good practice to have only 1 or 2 users in this role for any given group.

Group-level permissions may change what operations a user may perform within a group, but this is isolated to the designated group. So a user may be an administrator of one group and simply a member of another group. Groups are created and managed by the **site manager**.

For quick reference, see the table below for the roles and permissions within a group.

<table style="height: 388px;" width="714">
<tbody>
<tr>
<td><b>Role</b><p></p>
<p><em>(User Type)</em></p></td>
<td><b>Description</b></td>
<td><strong>Permissions </strong><p></p>
<p><em>(What can I do?)</em></p></td>
</tr>
<tr>
<td><b>Member:</b></td>
<td><span style="font-weight: 400;">A basic user within the group who is mostly adding and editing content for the group.</span></td>
<td>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Create, edit, and delete content they have created within their group.</span></li>
</ul>
</td>
</tr>
<tr>
<td><b>Administrator:</b></td>
<td><span style="font-weight: 400;">A role meant for one or two people to manage content created within a group. This higher level of permissions is restricted to the user’s group, so that a groups can work somewhat independently without compromising the larger site. </span></td>
<td>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Add and remove group members.</span></li>
</ul>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Manage permissions of group members.</span></li>
</ul>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Create, edit, delete all content within the group.</span></li>
</ul>
</td>
</tr>
</tbody>
</table>

We’re excited to include core roles and permissions as a standard feature included in our latest release of DKAN. You can learn more about the many feature enhancements, improvements, and fixes made in this release by reading the full [release notes](https://github.com/NuCivic/dkan/releases/tag/7.x-1.11) on our public GitHub [DKAN repository](https://github.com/NuCivic/dkan/releases/tag/untagged-2c42c7ba2e50803da9fe).

Have questions or thoughts? Let us know on our public [DKAN Repo](https://github.com/NuCivic/dkan) through [issues](https://github.com/NuCivic/dkan/issues) or chat with us in [our Gitter room](https://gitter.im/NuCivic/dkan?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge).
