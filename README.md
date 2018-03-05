
<p align="center">
  <br>
    <img src="https://www.cbd.int/app/images/cbd-logo-green-en.svg" width="400px"/>
  <br>
<img src="https://raw.githubusercontent.com/scbd/stacks/master/dev/drupal/drupal-scbd.png" width="150px"/> <br>
<a href="https://www.drupal.org/8">Drupal 8</a> Module
</p>
CONTENTS OF THIS FILE

---------------------

 * Introduction
 * Requirements
 * Installation
 * Configuration
 * How it works
 * Maintainers

INTRODUCTION
------------

Social Auth SCBD is a SCBD authentication integration for Drupal. It is
based on the Social Auth and Social API projects

It adds to the site:
 * A new url: /user/login/scbd.
 * A settings form on /admin/config/social-api/social-auth/scbd page.
 * An SCBD Logo in the Social Auth Login block.

REQUIREMENTS
------------

This module requires the following modules:

 * Social Auth (https://drupal.org/project/social_auth)
 * Social API (https://drupal.org/project/social_api)

INSTALLATION
------------

 * Run composer to install the dependencies.
   composer require "drupal/social_auth_scbd:~1.0"

 * Install the dependencies: Social API and Social Auth.

 * Install as you would normally install a contributed Drupal module. See:
   https://drupal.org/documentation/install/modules-themes/modules-8
   for further information.

CONFIGURATION
-------------

 * Add your SCBD project OAuth information in
   Configuration » User Authentication » SCBD.

 * Place a Social Auth SCBD block in Structure » Block Layout.

 * If you already have a Social Auth Login block in the site, rebuild the cache.


HOW IT WORKS
------------

User can click on the SCBD logo on the Social Auth Login block
You can also add a button or link anywhere on the site that points
to /user/login/scbd, so theming and customizing the button or link
is very flexible.

When the user opens the /user/login/scbd link, it automatically takes
user to SCBD Accounts for authentication. SCBD then returns the user to
Drupal site. If we have an existing Drupal user with the same email address
provided by SCBD, that user is logged in. Otherwise a new Drupal user is
created.


MAINTAINERS
-----------

Current maintainers:
 * <a href="https://github.com/scbd">UN Convention on Biological Diversity - https://github.com/scbd</a>
