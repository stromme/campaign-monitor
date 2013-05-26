campaign-monitor
================

WP PLUGIN Campaign monitor

This plugin syncs the wp users DB with a given campaign monitor subscriber list. Plugin should only load in wp-admin. Care should be taken to make the plugin as light as possible so as not to provide any further burden on wp-admin page load times.

## Network settings

Select which campaign monitor subscribers list to sync with.

## Adding / Removing Subscribers

Use the native wp action hooks for adding/removing user. When a user is added or removed in wp, add or remove the same person from the Campaign Monitor Subscribers list.

You'll likely have to add a new field to the subscribers list to contain either the wp user name or user ID.

## Updating a user

Use the wp hook called on user update to sync updates to the following fields with Campaign Monitor:

First Name
Last Name
Email




