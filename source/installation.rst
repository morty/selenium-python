.. _installation:

Installation
------------

Introduction
~~~~~~~~~~~~

Selenium Python bindings provides a simple API to write
functional/acceptance tests using Selenium WebDriver.  Through
Selenium Python API you can access all functionalities of Selenium
WebDriver in an intuitive way.

Selenium Python bindings provide a convenient API to access Selenium
WebDrivers like Firefox, Ie and Chrome.  The current supported Python
versions are Python 2.6 and Python 2.7.  Python 3 is not yet
supported.  Selenium server is a Java program.  Java Runtime
Environment (JRE) 1.6 is recommended to run Selenium server.  This
article explain using Selenium 2 with WebDriver API.  Selenium 1 API
is not covered here.


Downloading Selenium server
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. note::

  The Selenium server is only required, if you want to use the remote
  WebDriver.  See the :ref:`selenium-remote-webdriver` section
  for more details.

You can download Selenium server 2.x from the `download page of
selenium website <http://seleniumhq.org/download/>`_.  The file name
should be something like this:
``selenium-server-standalone-2.x.x.jar``.  You can always download the
latest 2.x version of Selenium server.

If Java Runtime Environment (JRE) is not installed in your system, you
can download the `JRE from the Oracle website
<http://www.oracle.com/technetwork/java/javase/downloads/index.html>`_.
If you have root access in your system, you can also use your
operating system instructions to install JRE.


Downloading Python bindings for Selenium
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can download Python bindings for Selenium from the `PyPI page for
selenium package <http://pypi.python.org/pypi/selenium>`_.  It has a
dependency on `rdflib <http://pypi.python.org/pypi/rdflib>`_ , version
3.1.x.

You can also use `easy_install
<http://python-distribute.org/distribute_setup.py>`_ or `pip
<http://pypi.python.org/pypi/pip>`_ to install the bindings::

  easy_install selenium

or::

  pip install selenium

You may consider using `virtualenv
<http://pypi.python.org/pypi/virtualenv>`_ to create isolated Python
environments.


Running Selenium server
~~~~~~~~~~~~~~~~~~~~~~~

You should have Java Runtime Environment (JRE) in the system.  If
`java` command is available in the PATH (environment variable), you
can start the Selenium server using the command command given below.
Replace `2.x.x` with actual version of Selenium server you downloaded
from the site.  If JRE is installed as a non-root user and/or if it is
not available in the PATH (environment variable), you can type the
relative/absolute path to the `java` command, for eg:-
``./jre1.6.0_26/bin/java``::

  java -jar selenium-server-standalone-2.x.x.jar

