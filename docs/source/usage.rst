Usage Guide
===========

This page provides information on how to use and extend this documentation.

Document Structure
------------------

The documentation is organized as follows:

* ``index.rst`` - Main landing page with table of contents
* ``installation.rst`` - Installation and setup instructions
* ``usage.rst`` - This usage guide
* ``conf.py`` - Sphinx configuration file

Writing Documentation
---------------------

This documentation uses reStructuredText (reST) format. Here are some common
formatting examples.

Headers
~~~~~~~

Use underlines to create headers::

   Main Title
   ==========

   Section
   -------

   Subsection
   ~~~~~~~~~~

Text Formatting
~~~~~~~~~~~~~~~

You can format text in various ways:

* *Italic text* - use ``*italic*``
* **Bold text** - use ``**bold**``
* ``Code text`` - use double backticks

Lists
~~~~~

Bullet lists::

   * First item
   * Second item
   * Third item

Numbered lists::

   1. First item
   2. Second item
   3. Third item

Code Blocks
~~~~~~~~~~~

Use the ``code-block`` directive for syntax-highlighted code:

.. code-block:: python

   def hello_world():
       """A simple function."""
       print("Hello, World!")
       return True

Links
~~~~~

Internal links to other pages:

* :doc:`installation` - Link to installation page
* :doc:`index` - Link to index page

External links:

* `Sphinx Documentation <https://www.sphinx-doc.org/>`_
* `reStructuredText Primer <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_

Adding New Pages
----------------

To add a new documentation page:

1. Create a new ``.rst`` file in the ``docs/source`` directory
2. Add content using reStructuredText syntax
3. Add the page to the ``toctree`` in ``index.rst``
4. Rebuild the documentation

Example
~~~~~~~

To add a new page called "examples.rst":

1. Create ``docs/source/examples.rst``
2. Add it to the toctree in ``index.rst``::

      .. toctree::
         :maxdepth: 2

         installation
         usage
         examples

3. Build: ``sphinx-build -b html source build``

Rebuilding
----------

After making changes to any documentation files, rebuild to see the updates:

.. code-block:: bash

   cd docs
   sphinx-build -b html source build

Then open ``docs/build/index.html`` in your web browser to view the changes.
