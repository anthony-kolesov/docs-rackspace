============================
Style guide revision history
============================

This file summarizes the changes that have been made to the style guide.

November 10, 2016
~~~~~~~~~~~~~~~~~

-  Converted the style guide to reStructuredText.
-  :ref:`trademarks`: Added guidelines to show the term *Fanatical Support* in
   bold and italics (using the ``:bolditalic:`` directive in RST) and to show a
   registered trademark symbol on first use.

July 27, 2016
~~~~~~~~~~~~~

-  Updated the *README* and *index* files to add Rackspace Private Cloud
   contributors as consumers of the style guide.

-  :ref:`alphabetical-list-of-terms`:

   -  *be sure*: Added guidelines to avoid it and use *ensure* or *verify*
      instead.
   -  *data store*: Changed guidelines from one word to two words.
   -  *dialog*: Added guideline to avoid it, and referred to *dialog box*.

-  :ref:`commas-in-numbers`: Revised to use a comma in five-digit numbers,
   rather than 4-digit numbers, to follow IBM and OpenStack guidelines.

-  :ref:`ellipses`: Added a caveat that writers can include an ellipsis with a
   UI label if omitting it would cause confusion.

-  :ref:`placeholder-text`: Revised guidelines to use ``:samp:`` directive in
   RST.

-  :ref:`text-formatting`: Updated guidelines to use RST directives when
   available, and noted style differences between Public and Private Cloud.

   -  Command names: Use monospace for Public, apply the ``:command:``
      directive (bold) for Private.
   -  Directory names, file names, paths: Use bold for Public, monospace
      for Private.
   -  Glossary terms: In RST, apply the ``:term:`` directive.
   -  GUI labels: In RST, apply the ``:guilabel:`` directive.
   -  Keyboard keys: Use bold for Public, monospace for Private.
   -  Menu sequences: In RST, apply the ``:menuselection:`` directive.
   -  Option names: In RST, apply the ``:option:`` directive.
   -  Parameter names: In RST, apply the ``:option:`` directive.
