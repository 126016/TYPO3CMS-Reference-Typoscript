.. include:: ../Includes.txt


.. _typoscript-syntax-templates-debugging:
.. _typoscript-syntax-debugging:

Debugging
^^^^^^^^^

There are no tools that will tell you that your TypoScript code is
100% correct. The TypoScript Object Browser will warn you about syntax errors
though:

.. figure:: ../Images/TemplatesSyntaxError.png
   :alt: The TypoScript Object Browser showing a syntax error


Errors will also appear in the Template Analyzer, when viewing the
content of a give template. It is also possible to see the full
TypoScript code by clicking on the "View the complete TS listing"
button at the bottom of the Template Analyzer:

.. figure:: ../Images/TemplatesViewFullListingButton.png
   :alt: The TypoScript Object Browser showing a syntax error


The result is a long listing with all compiled line numbers, which
makes it easy to find the error reported by the TypoScript Object Browser.

.. figure:: ../Images/TemplatesFullListing.png
   :alt: The TypoScript Object Browser showing a syntax error


In the frontend, the Admin Panel is another possibility to debug
TypoScript; use its section called "TypoScript"! It shows you selected
rendered (configuration) values, SQL queries, error messages and more.

TypoScript itself offers a number of debug functions:

- :ref:`stdWrap <stdwrap>` comes with the properties
  :ref:`debug <stdwrap-debug>`, :ref:`debugFunc <stdwrap-debugfunc>` and
  :ref:`debugData <stdwrap-debugdata>` which help checking which values
  are currently available and which configuration is being handled.

- :ref:`GMENU <gmenu>`, :ref:`TMENU <tmenu>` and
  :ref:`IMGMENU <imgmenu>` come with the property
  :ref:`debugItemConf <menu-common-properties>`. If set
  to "1", it outputs the configuration arrays for each menu item.
  Useful to debug :ref:`optionSplit <objects-optionsplit>`
  things and such.
