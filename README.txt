Administer Users by Role
========================

This module allows site builders to set up fine-grained permissions for
allowing "sub-admin" users to edit and delete other users — more specific
than Drupal Core's all-or-nothing 'administer users' permission. It also
provides and enforces a 'create users' permission.

Pre-Release Information
-----------------------

This is a pre-release of the Administer Users by Role module. We are currently seeking testers,
feedback, and co-maintainers.

All 1.x-0.1.x tags will be used to denote pre-release status. The first
official release will be numbered 1.x-1.1.0.

Core Permissions
----------------

Administer users
  DO NOT set this for sub-admins.  This permission bypasses all of the
  permissions in "Administer Users by Role".

View user profiles
  Your sub-admins should probably have this permission.  (Most things work
  without it, but for example with a View showing users, the user name
  will only become a link if this permission is set.)

Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules

New Permissions
---------------

Access the users overview page
  See the list of users at admin/people.  Only users that can be edited are shown.

Create new users
  Create users, at admin/people/create.

Edit users with no custom roles
  Allows editing of any authenticated user that has no custom roles set.

Edit users with role XXX
  Allows editing of any authenticated user with the specified role.
  To edit a user with multiple roles, the sub-admin must have permission to
  edit ALL of those roles.  ("Edit users with no custom roles" is NOT needed.)

The permission for cancel work exactly the same as those for edit.

Issues
------

Bugs and Feature requests should be reported in the Issue Queue:
https://github.com/kelizoliva/administerusersbyrole/issues

Current Maintainers
-------------------

- Kristin Snelling (https://github.com/kelizoliva).
- Seeking additional maintainers.

Credits
-------

- Ported to Backdrop CMS by Kristin Snelling (https://github.com/kelizoliva).
- Maintained for Drupal by Adam Shepherd (https://www.drupal.org/u/adamps).
- Maintained for Drupal by Tom Kirkpatrick (https://www.drupal.org/u/mrfelton).
- Maintained for Drupal by Steve Mokris (https://www.drupal.org/u/smokris).
- Ongoing Drupal development sponsored by AlbanyWeb.
- Initial Drupal development sponsored by Kosada.


