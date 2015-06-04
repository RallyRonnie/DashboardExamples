Sprint Planning Dashboard
=========================

## Overview
This is example of real-time updates between 2 APPs. It consists of a new custom list app
on the left and a custom Burnup app on the right that renders a burnup when a PortfolioItem
is selected on the left. This is used by initiative owners, POs, PMs to status at the program
level.

Construction Instructions:
* Create a new Page called "Feature|Epic|Initiative Burnup Dashboard" - base name on PI level used
* You can make it a Release scoped page or not, where you might add a Query to filter PIs.
* Set Page format to 2 column, left narrow, right wide.
* Add APP Catalog "Custom List" to left column.
* Set title to something like "Current PI Features" or whatever PI scope you are displaying
* (Optional) if you didn't use a Released scoped page, add a query like: ((Release.StartDate <= today) AND (Release.ReleaseDate >= today)) for the current release. NOTE: this will only work on the lowest level Portfolio Item type.
* Add APP Catalog "Custom HTML" to right column.
* Paste code from https://github.com/RallyRonnie/PIBurnupFromSelect/blob/master/deploy/App.html into the HTML box.
* Set "Title" to "Burnup Chart" for example.
* Save

## Screen Shot

![Team Board Example](https://raw.github.com/RallyRonnie/DashboardTest/master/PIBurnupDashboard.png)
