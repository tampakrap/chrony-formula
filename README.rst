======
chrony
======

Formula to set up and configure chrony

Available states
================

.. contents::
    :local:

``chrony``
----------

Installs the chrony package.

``chrony.config``
-----------------
This state manages the file ``chrony.conf`` under ``/etc`` (template found in "chrony/files"). The configuration is populated by values in "chrony/map.jinja" based on the package's default values (and RedHat, Debian, Suse and Arch family distribution specific values), which can then be overridden by values of the same name in pillar.

``chrony.removed``
-----------------
Stops the service and uninstalls the package.
