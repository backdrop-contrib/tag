Tag Module
==========

The Tag module provides two basic components:

- A mechanism to suggest tags for an entity being saved.  Modules wanting 
to provide tag suggestions should implement hook_tag_suggestion_info() - see 
tag.api.php
- A mechanism to do something with the tags suggested by each "suggestion" 
module.  A module wanting to react to changes in tags (e.g. provide a user 
interface), should implement hook_tag_ui_info() - again, see tag.api.php

A basic "Tag-on-save" module is included with the Tag API module.  This module 
provides the basic functionality of adding ALL tags suggested by a suggestion 
module when an entity is saved.  This, along with the 7.x-3.0 branch of the 
should serve as examples to get 
started with the Tag API.

* Issues

The Tag module currently only works with the Node entity type, although 
it could easily be altered to work with any entity type.  If somebody is keen 
to get this working with other entities, I'd certainly accept help/patches.

REQUIREMENTS
------------

None.

RECOMMENDED MODULES
-------------------

- Autotag module (http://backdrop.org/project/autotag)

INSTALLATION
------------

Install only if required by another module.

CONFIGURATION
-------------

The module has no menu or modifiable settings.  There is no
configuration. 


LICENSE
---------------    

This project is GPL v2 software. See the LICENSE.txt file in this directory 
for complete text.

MAINTAINERS
-----------

Current maintainers:

* Wilmoth Shillingford (docwilmot) - https://github.com/docwilmot

CREDIT
-----------

Original maintainer:

* Simon Rycroft (sdrycroft) - https://www.drupal.org/user/151544
