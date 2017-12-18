# Ultimate Theming for Jira Service Desk

## Introduction

This is the documentation and help page for the new version 2.X of the Ultimate Theming for Jira Service Desk.

You can find the old documentation for v.1.X [here](https://pronto-plugins.herokuapp.com/ultimate.html).

## What changed from version 1 to version 2

* Added the option to customize login page
* Added the option to export to Excel from "My requests".
* Made the request view of a portal isolated, meaning that a theme can be applied to the "request types" view of a portal, and another theme can be applied to the "request view" of a portal.
* A new structure for the server side, meaning the themes from v1 is going to be migrated into a new format going forward. You should only notice some visual changes to modal windows and so on if updating the plugin.
* New users must create a theme and assign it to a portal page, before any customization can be made. A layout must be added to the theme as well, if one wants to change the structure of a portal page.

More features are to be added soon.

## Features

* IN APP editor, which means live editing by Administrator in the Service Desk.
* Create/edit/apply themes. A theme is applied to Service Desk location, e.g. the Portals page, a specific desk/portal, the user profile and so on. A theme consist of layout, custom HTML, uploaded files and changes to UI components.
* Create/edit/apply layouts to themes: insert custom HTML in layout areas using a rich text editor, link to uploaded files, and insert images.
*Upload files - for a theme. Javascript and CSS are automatically loaded when a theme loads. Events in your javascript can be triggered on location change!
* Edit (and hide) different components in the Service Desk:
* Create a category view of portals that replaces the normal portals view.
* Hide different groups and requests types, and hide them from search.
* Add fields to the “My Requests” form, e.g. Created/Updated/Labels and more.
* Customize login page.
* Export to Excel from "My requests".

## Installation

Installation in Jira is through Atlassian Marketplace, or by downloading a version and uploading into the Addons section of Jira. 

## Usage 

1. As as administrator (or Sysadmin) go to the portals.
2. Click the "Ultimate themning" button in the bottom right corner. A left side menu bar should show up.

## Explanation

### Themes

<a name="themes"></a>

The plugin is theme-based, which means that every Service Desk page is under a theme. Beware that for portals, the request view is also

**By default all pages have no theme assigned.**

All customizations you make (except changing the global footer) are *bound to a theme*. This means themes can be re-used all over the portal. This also means you can have different views on different portal pages - maybe you need to print guidelines on one portal, and show some links on another. Theming lets you do that.

Uploads are only usable on pages for the theme they were uploaded to. For instance, .cs/.js files, will only be rendered to the specific theme.

### Layouts
A layout defines the structure of the page. 

**When no layout is assigned to the theme of the current portal page, the layout is just Service Desk "as is".**

By creating and assigning a layout, you can have top/bottom/sidebars/custom areas for inserting your own HTML.

The HTML is edited in raw source code. So make sure write valid HTML. E.g. put it through a HTML validator before using it.

Layouts can be created in the modal window for managing layouts. Just click the button next to "Layouts:" in the menu bar. Remember, you have to assign a theme first (as layouts are bound to them). You can also edit, copy or delete layouts. Clicking the assign button next to a layout, assigns the layout to the current theme. 

Layouts can have editable areas. By creating those, you can click the pencil icon at the area (when the layout is set on the theme) and use a simple WYSIWYG HTML editor to add content, like uploaded images etc.

Editable areas are created using the macro **${editable}** in the HTML. This creates a wrapping div when rendered.


### Uploads

