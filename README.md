Description
===========

Install perforce with a config file sourced in .bash_profile

Requirements
============

Chef 10

Attributes
==========

* p4
** owner - System user in who's home directory the configs will be stored. File permissions use this user as well.
** group - System group of the owner above.
** port  - Perforce server (eg. perforce-server:1666)
** user  - Perforce user. Defaults to owner.
** password - Perforce password.
** diff
** editor
** merge
** client
** charset
** commandcharset
** language
** host

Usage
=====

Include the recipe and set the attributes above as node or environment attributes

    include_recipe 'perforce'