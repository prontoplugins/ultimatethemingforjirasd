## Ultimate Theming for Jira Service Desk

<img src="logo.png" width="200" />

## Introduction

This is the documentation and help page for the new version 3.X of the Ultimate Theming for Jira Service Desk.

You can find the old documentation for v.2.X [here](https://prontoplugins.github.io/ultimatethemingforjirasd/v2).
You can find the old documentation for v.1.X [here](https://pronto-plugins.herokuapp.com/ultimate.html).

## What changed from version 2 to version 3

* Added modular approach for building content (with content+sidebars or a customized grid). Removed functionality of themes.
* Added full sorting of fields in ”Requests”.
* Added fields to filter on in ”Requests”.
* Improved fetch of SLA info.
* Improved the generation of CSV in ”Requests”.
* Edit ”Sign up” and ”Knowledge base” pages.
* Added global JavaScript/CSS
* global files (can always be linked to from every page)

## Features

* IN APP editor, which means live editing by Administrator in the Service Desk. (When you go to the service desk, a top bar is added for admins)
* Create/edit layout, content and design any portal page in Service Desk. If you enable the module based design, a portal page can be edited with rows, columns and modules.
* Requests page module can be extended with additional fields (sorting as well).
* Requests page module can be extended with additional search fields (labels, reporter and custom selects).
* CSV export can be enabled on the Requests page
* Request page (details of a request) can be extended to show additional fields.
* Portals (list of portals) can be changed to show a category tab-view of portals.
* Modules that can be inserted as well includes: HTML (upload images, or link to files), announcement, search bar, recent portals, popular portals (where applicable).
* Global JavaScript/CSS. JavaScript is executed on page view, and css is injected automatically.
* Theme login, signup and knowledge base pages!

## Installation

Installation in Jira is through Atlassian Marketplace, or by downloading a version and uploading into the Addons section of Jira. 

## Getting started
As as administrator (or Sysadmin) go to the portals.

First of, things will look different than in version 2. The right side menu is gone, and a top bar is shown instead. The theming part is gone. Now you edit all pages as they are. You dont set a layout anymore, but instead you build up pages with rows and columns of modules.

You can still edit the main module of a page (where applicable). For instance, on /portals, you can set categories of portals, or in user/requests you can add fields.

When you first go to a page (e.g. portals), you cannot edit the actual layout. To do this, you must change design for the page. Go to the ”More” menu and click ”Change design”. Change to ”Module based”. Click OK. The design and layout will now change a bit, and an ”Edit” button is now visible. Click Edit. The main content area is now changed into a layout/content editor. You can add rows, modules and edit the modules. You can change the layout of the rows by click Columns. Here you can choose between content+sidebars, or a custom columned-row (responsive options).

Click add module in a column to add a module. By default, the main module (context defined) is already added. Modules available are: primary module (by context), and modules like search bar, HTML, breadcrumb, and announcement. On /portals, you can add modules like ”recent” and ”popular”. Those fits nicely with e.g. category based view of the portals. You can always edit the configuration of a module (where applicable).

You can also move modules around (just drag the header part). And you can add new rows as well.

When editing, a Versions button is also visible. Here you can go back to another version from earlier time. And dont worry, if you edit something wrongly, you can cancel out (button next to versions).

Note that the edit of the main module is always possible (where applicable), even if you did not change into ”Modules based” design.

## Global JavaScript/CSS
In the ”More” menu click on Global JavaScript/CSS. Define as you like. We recommend you make sure the stuff is valid before saving it.
On every page change, the javascript is re-executed. To get the location of the user: check out the global js variable ”window.ULTIMATE_SERVICEDESK_LOCATION”.
The CSS is automatically injected.

## Manage files (uploads)
Uploads are now visible for all pages and not limited to a theme as before. Use the HTML-module to show e.g. an image, or link to a file.

## Edit of login page and signup pages
In Service Desk, there is a global login/signup page, and a login/signup page for each portal.
To edit the login page of a portal (or /portals for global), go the portal (or /portals) page, then go to the ”More” menu, and click ”Edit login page.” Now you are actually signed out, but still able to edit the page. If you have enabled public signup, you can even click the signup link, and edit that page as well. Sign in again to continue editing the ”restricted” pages.

## The Requests page (my requests, all requests or organisation requests)
On the requests page it’s possible to add additionals fields (as columns) to the table of requests. The fields will be sortable (if applicable).  A bunch of field types are possible to add. Please reach out, if you find something missing.

You can also add additionals fields to search for (filtering). Right now requester/reporter, labels and the custom field type of select are possible to add.

Finally, you can enable CSV export button. Here it’s possible to export current shown issues, or all issues that the filtering matches. Values of additional fields are also exported.

## Categories of portals
Go to the /portals page. Click edit below the list of portals. (Or if you have enabled ”Module based” design, you first need to click Edit in the top, before you can edit the module.)
A window opens where you can group the portals into categories, and then the portals are shown in a tab view instead. You can sort the portals to change the order of things. Other options are also available.

## Request view
Here it’s possible to add additional fields as well.

## Future
For 3.1 we will be adding a custom design, that is built to support the module approach in a more consistent way. The design will be editable wrt. colors, so you can brand it.

We will also be adding a way to template pages, so you can reuse layouts around the portal area.




