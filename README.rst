REST Emailer Plug-in
====================

.. image:: https://travis-ci.org/curityio/emailer-rest-plugin.svg?branch=dev
     :target: https://travis-ci.org/curityio/emailer-rest-plugin

This project provides an open source email plugin for the Curity Identity Server. The only functionality of this plugin is to print the email to be sent to the log on info level.

System Requirements
~~~~~~~~~~~~~~~~~~~
* Curity Identity Server 6.0.0 and `its system requirements <https://developer.curity.io/docs/latest/system-admin-guide/system-requirements.html>`_

Requirements for Building from Source
"""""""""""""""""""""""""""""""""""""
* Java JDK v. 8

Compiling the Plug-in from Source
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The project can be built using gradle. Use the command ``gradle build`` to find the resulting JARs in the ``build/libs`` directory.

Installation
~~~~~~~~~~~~
To install the plugin, you need the binary files. You can build these yourself, as described in the previous section.

Take the resulting JAR-files and copy them into the directory ``${IDSVR_HOME}/usr/share/plugins/noopmailer``.

Note that the ``/noopmailer`` directory can be named freely; using (a reference to) the name of the plugin just makes it
easier to find the files later on.

The plugin will become available after you (re)start the Curity Identity Server.

.. note::

    The JAR file needs to be deployed to each run-time node and the admin node. For simple test deployments where the admin node is a run-time node, the JAR file only needs to be copied to one location.

For a more detailed explanation of installing plug-ins, refer to the `Curity developer guide <https://developer.curity.io/docs/latest/developer-guide/plugins/index.html#plugin-installation>`_.

License
~~~~~~~

This plugin and its associated documentation is listed under the `Apache 2 license <LICENSE>`_.

More Information
~~~~~~~~~~~~~~~~

Please visit `curity.io <https://curity.io/>`_ for more information about the Curity Identity Server.

Copyright (C) 2021 Curity AB.

