Installation
============

This page describes how to install and set up the documentation build system.

Prerequisites
-------------

Before building the documentation, ensure you have the following installed:

* Python 3.7 or higher
* pip (Python package manager)

Installing Sphinx
-----------------

To build this documentation, you need to install Sphinx and its dependencies.

Using pip
~~~~~~~~~

Install Sphinx using pip:

.. code-block:: bash

   pip install sphinx

Or install from the requirements file:

.. code-block:: bash

   pip install -r requirements.txt

Verifying Installation
----------------------

To verify that Sphinx is installed correctly, run:

.. code-block:: bash

   sphinx-build --version

You should see output similar to::

   sphinx-build 9.0.4

Building the Documentation
---------------------------

Once Sphinx is installed, you can build the documentation using:

.. code-block:: bash

   cd docs
   sphinx-build -b html source build

The generated HTML files will be in the ``docs/build`` directory.

Alternative: Using Make
~~~~~~~~~~~~~~~~~~~~~~~

If you have a Makefile, you can also build using:

.. code-block:: bash

   cd docs
   make html

Next Steps
----------

Now that you have the documentation built, see the :doc:`usage` page to learn
how to use and extend this documentation.
