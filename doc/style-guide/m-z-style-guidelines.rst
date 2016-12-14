.. _mz-style-reference:

===================
M-Z style reference
===================

This section of the writing style guide provides detailed guidelines
about and instructions for applying style conventions. For more
guidelines, see `A-L style reference <al-style-reference>`.

-  `Messages <#messages>`__
-  `Names <#names>`__
-  `Notes and other notation types <#notes-and-other-notation-types>`__
-  `Numbers <#numbers>`__
-  `Parameters <#parameters>`__
-  `Placeholder (variable) text <#placeholder-variable-text>`__
-  `Plurals <#plurals>`__
-  `Product names and version
   numbers <#product-names-and-version-numbers>`__
-  `Punctuation <#punctuation>`__
-  `Symbols <#symbols>`__
-  `Tables <#tables>`__
-  `Tasks and procedures <#tasks-and-procedures>`__
-  `Telephone numbers <#telephone-numbers>`__
-  `Text formatting <#text-formatting>`__
-  `Time <#time>`__
-  `Titles and headings <#titles-and-headings>`__
-  `Trademarks <#trademarks>`__
-  `URLs and domain names <#urls-and-domain-names>`__

Messages
~~~~~~~~

If you help write the message text for a product or you suggest edits to
message text, use the guidelines in this topic.

.. note::

   Change message text *only* at the request of (or as a
   suggestion to) the developer. When citing message text in a document,
   cite the text that the user sees in the product.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Guideline
     - Example
     - Comments
   * - Use complete sentences, when possible.
     - *Use:*

       The authentication token is not valid.

       *Avoid:*

       Invalid authentication token
     - Include articles (*a*, *an*, *the*) to make the sentence complete. If
       possible, use active voice.

       .. note::

          Message text that serves as a heading or label (such as
          ``Elapsed:hh:mm:ss``, which indicates elapsed time) is acceptable as
          a fragment.
   * - Use more than one sentence if required for clarity.
     - You must provide a name for each domain. null is not a valid domain
       name.
     - Write brief and simple sentences that clearly state the problem.
       Separate the sentences with a period (or question mark, if applicable),
       not with a semicolon.
   * - Avoid using only uppercase letters.
     - *Use:*

       The requested image $UUID has automatic disk resizing disabled.

       *Avoid:*

       THE REQUESTED IMAGE $UUID HAS AUTOMATIC DISK RESIZING DISABLED.
     - Lines with excessive capitalization are hard to read. Use all uppercase
       letters only for words that require it, such as a keyword, a data type,
       or a specific table name that is displayed in all uppercase letters to a
       database user.
   * - When possible, include a recommendation, either a potential fix or a
       reference to a document for more information.
     - The system is out of virtual IP addresses. Contact Support so they can
       allocate more virtual IP addresses.

       The value -1.0 cannot be accepted. Specify a positive integer value for
       the volume size.
     - Messages should provide specific information about how the user should
       continue.
   * - Be specific.
     - *Use:*

       The live migration of instance 89a5e582-d3f3-4665-ate2-03c2114f0bib to
       host compute2 failed.

       *Avoid:*

       Live migration failed.
     - Messages should provide as much detailed information as possible.
   * - Use *n* to represent an unspecified or generic number. Use *x* to
       represent an unknown version number.
     - The rate limit has been reached (*n* requests in 24 hours). Please try
       again later.

       This option is available only for Ubuntu 12.\ *x*.
     - None
   * - Avoid blaming the user.
     - *Use:*

       The request could not be understood by the server because of malformed
       syntax.

       *Avoid:*

       You entered bad request syntax.
     - Rewrite messages that imply fault on the part of the user. Use passive
       voice when necessary.
   * - When possible, use positive statements.
     - *Use:*

       The given limit must be positive and must be less than 50.

       *Avoid:*

       The given limit cannot be negative and cannot be greater than 50.
     - Positive statements are easier to understand than negative statements.

Names
~~~~~

Do not use real or copyrighted names in examples. For example, do not
use kelly.holcomb@example.com.

See the following topics for information about product names:

- `Product names and version number <#product-names-and-version-numbers>`__
- `Third-party names and trademarks
  <../terminology-guidelines.html#third-party-names-and-trademarks>`__

Notes and other notation types
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Notations (notes, tips, and warnings) call out important or helpful
information. Use them sparingly, according to the guidelines in the
following table.

.. list-table::
   :widths: 30 70
   :header-rows: 1

   * - Notation type
     - Description
   * - Important
     - Presents an important or essential point. As a rule, customers must pay
       attention to important notations to complete a task or understand a
       topic.
   * - Note
     - Provides information that emphasizes or supplements information in the
       text. A note can provide information that applies only in certain cases.
   * - Tip
     - Provides useful information that might improve product performance or
       make procedures easier to follow. Tips provide the following benefits:

       • Help customers learn techniques or procedures
       • Show alternative ways of doing something
       • Provide shortcuts
       • Provide helpful (but not essential) information

   * - Warning
     - Alerts customers to potential hazards or highlights critical
       information. Use a warning for situations in which users could lose
       data, compromise data integrity, or disrupt operations if they do not
       follow instructions carefully.

When creating notations, use the following guidelines:

-  Use the style or element in your authoring tool to create the
   notation. If there is no style or element, create the notation as
   follows: Type the word **Important**, **Note**, **Tip**, or
   **Warning**, follow it with a colon, make both the label and the
   colon bold, and then provide the text of the notation in regular
   font. If a notation contains more than one item (such as two notes
   presented in a unordered list), make the label plural (for example,
   **Notes**).

-  Place a notation as close as possible to the information that it
   emphasizes or clarifies.

-  Do not "stack" notations of the same type (for example, by following
   one labeled note directly with another labeled note). Instead, use
   separate paragraphs or an unordered list within a single notation. It
   is acceptable for notations of different types to follow one another.

Numbers
~~~~~~~

Use the following guidelines for showing numbers in documentation.

-  `Numbers versus words <#numbers-versus-words>`__
-  `Commas in numbers <#commas-in-numbers>`__
-  `Ranges of numbers <#ranges-of-numbers>`__
-  `Unspecified, generic, and unknown
   numbers <#unspecified-generic-and-unknown-numbers>`__

Numbers versus words
--------------------

Spell out numbers from zero through nine, except in the cases shown in
the following table. In these cases, or if the number is 10 or larger,
use numerals.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Exception
     - Example
   * - Numbers as they are displayed
     - The returned value is 0.
   * - Numbers to use as input
     - Type **1** and press **Enter**.
   * - Series of the same type of items where at least one of the numbers is
       greater than nine
     - Unit A requires 5 nodes, Unit B requires 17 nodes, and Unit C requires 9
       nodes.
   * - Numbers with symbols
     - 7%
   * - Numbers with units of measure or abbreviations
     - 5 mm, 3-inch disk
   * - Numbers that indicate dimensions
     - 8x8 feet
   * - Time
     - 5:45 p.m.

Avoid beginning a sentence with a number. If you must begin a sentence
with a number, spell out the number unless the number is part of a
product, service, or company name.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - Ten vendors, including Rackspace, were assessed based on the following
       attributes:

       451 Research applied a weighting system to highlight the attributes that
       are most valued by end users.

Do not use the spelled-out form of a number followed by a numeral in
parentheses. However, if you think that a user might misread the numeral
0 as the letter O, you can clarify by spelling out zero parenthetically
after the numeral.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - two panels

       zero probability

       Enter **0** (zero). *(acceptable)*
     - two (2) panels

       zero (0) probability

Commas in numbers
-----------------

Use commas in numbers with five or more digits. However, do not use
commas in the following types of numbers:

- Addresses
- Fractional part of a decimal number
- Page numbers
- Literal representations of user-entered values or displayed values

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - 9001 N IH 35

       1452.7532

       page 1055

       1024 bytes
     - 9,001 N IH 35

       1,452.753,2

       page 1,055

       1,024 bytes

.. note::

   Do not use European-style numbering, which uses commas in the
   place of periods. For example, use 3.14159, not 3,14159.

Ranges of numbers
-----------------

When describing number ranges, use the following guidelines:

- To describe an inclusive range, use *through*. When space is limited, use an
  en dash instead. Do not use the word *inclusive* in your description.

- Use prepositions as follows:

  - If you use *between* to introduce a range, use *and* to conclude the
    range. Using *between* and *and* implies a noninclusive range.
  - If you use *from* to introduce a range, use *through* or *to* to
    conclude the range.
  - Do not mix *between* or *from* with an en dash.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - step 12 through step 16
       options 11–15 *(limited space)*
       any value from 1 through 258
     - step 12 through step 16, inclusive
   * - from 10 to 20 diagrams
     - from 10–20 diagrams
   * - between 2010 and 2012
     - between 2000–2002

Unspecified, generic, and unknown numbers
-----------------------------------------

To represent an unspecified or generic number, use *n* as the variable
and apply italics.

To represent an unspecified or unknown version number, use *x* for each
digit and apply italics.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - Move the insertion point *n* spaces to the right.

       Select the **Use *n* I/O Sessions** check box.

       Your BlackBerry software must be version 4.\ *x*.

Parameters
~~~~~~~~~~

When documenting parameters, observe the following guidelines:

-  In request and response examples, show all of the parameters.

-  Describe all of the parameters in tables preceding the examples.
   Observe the following guidelines for writing descriptions:

   -  Provide meaningful information about the parameter; don't just repeat
      the parameter's name. Link to other sections of the documentation if
      more explanation is needed or if the list of possible values is long.

   -  Write the first sentence of a description with an implied subject.
      For example, if the parameter is ``name``, the description might be
      "Server name, which becomes the initial host name of the server."

   -  Include any valid values and default value at the end of the
      description. Use the formats "Valid values are *n* and *n*." and "The
      default is *n*." For example, "Valid values are ``true`` and
      ``false``." and "The default is ``false``."

-  For request body parameters only, label the required parameters by
   adding the *(Required)* qualifier to the beginning of the
   description. For example:

   *(Required)* Path of the parameter to update. Valid values are
   ``/enabled``, ``/vault/region``, ``/vault/use_internal``, and
   ``/log-level``.

   Do not label optional request body parameters. Also, do not label URI,
   query, or response body parameters as either optional or required.

-  When listing and describing request and response body parameters in
   tables, show the parameters in the same order as they are shown in
   the examples. If you have more than one example, match the order in
   the first example shown.

-  Format parameter names in text according to the guidelines in `Text
   formatting <#text-formatting>`__.

Placeholder (variable) text
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Placeholder text (also referred to as variable text or replaceable text)
stands for an object whose specific name is unknown to us. Placeholders
are included when documenting syntax for how a command or path should be
constructed. Customers supply the relevant value for the placeholder
when using the command or syntax.

Placeholder text usually indicates the type of element that is being
represented. For example, *directoryName* would likely indicate the name
of a directory.

.. note::

   Placeholder text is distinct from *environment variables*.
   Environment variables have established formats and names, such as
   ``$account``, and their values are set in the system by customers and
   used consistently. By contrast, a placeholder is given a relevant value
   by the customer at the time that the customer runs the code or types the
   path. For information about formatting environment variables, see `Text
   formatting <#text-formatting>`__.

When creating placeholder text, use the following guidelines.

.. note::

   For specific information about showing placeholders for
   account information such as account numbers, user names, passwords, and
   API keys, see `Cloud account
   information <../a-l-style-guidelines.html#cloud-account-information>`__.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guidelines
     - Example
   * - Within regular text, show placeholder text in italics.

       Within code samples, use the RST ``:samp:`` directive, and enclose the
       placeholder text in curly braces. This formatting renders the
       placeholder in italics.

       If you cannot apply text formatting to the code, enclose placeholders in
       punctuation that does not have any other special use in the code. For
       example, use angle brackets or curly braces. Use a consistent convention
       throughout the documentation set.
     - :samp:`nova boot {serverName} --image {image} --flavor {flavor} --nic
       net-id=net1_id`
   * - Use lowercase letters except when showing a multiple-word placeholder.

       To show a multiple-word placeholder, do not separate the words with
       spaces or symbols. To distinguish the words in the placeholder,
       capitalize the first letter of each word after the first word (called
       camelCase). Do not capitalize the first word.

       .. note::

          Use lowercase and camelCase unless you have to follow the
          conventions of the programming language. For example, you might need
          to use underscores (account\_ID) or all capitals (ACCOUNT\_ID).
     - *password* *serverName* *apiKey* *tenantId*
   * - In general, use one or more whole words to represent a placeholder. Do
       not sacrifice clarity for brevity. Create placeholders that are
       descriptive and meaningful.
     - *device* (instead of *dev*)

       *installationDirectory* (instead of *installDir*)

       *mode* (instead of *########*)

When explaining a placeholder, use the following guidelines.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guidelines
     - Example
   * - Avoid stand-alone clauses that begin with *where*. Instead, use a
       sentence.
     - *Use:*

       **https://dfw.bigdata.api.rackspacecloud.com/v1.0/yourAccountId/**

       *yourAccountId* is your actual account number, which is returned as part
       of the authentication service response.

       *Avoid:*

       **https://dfw.bigdata.api.rackspacecloud.com/v1.0/yourAccountId/**

       where *yourAccountId* is your actual account number, which is returned
       as part of the authentication service response.
   * - If you need to explain two or more placeholders, use an unordered list.
     - From a supported web browser, type the following URL:

       **http://hostName:portNumber/ed/index.html**

       The placeholders in the URL are defined as follows:

       • *hostName* is the name of the host computer on which the application
         server is installed.

       • *portNumber* is the port number assigned to the application server.
         The default is 8082.
   * - Show the placeholder in regular text with the same formatting that it is
       shown in the path or code. For example, if you can show it in italics,
       use italics when explaining it. If you first show the placeholder in a
       code block and need to enclose it in angle brackets, show it in angle
       brackets and monospace when explaining it.
     - *Use:*

       **https://dfw.bigdata.api.rackspacecloud.com/v1.0/yourAccountId/**

       *yourAccountId* is your actual account number, which is returned as part
       of the authentication service response.

       *Use:*

       Run the following command, replacing ``<dockerHostName>`` with the name
       of your Docker host:

       ``docker-machine env <dockerHostName> --shell cmd``

Plurals
~~~~~~~

Use the following general guidelines for forming and using plurals. To
find out how to form the plural of a particular word, or for information
about whether to use the singular or plural form of a particular word,
see `Terminology <terminology-guidelines.md>`__ or consult a dictionary.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - To form the plural of an abbreviation, an acronym, or a number, add a
       lowercase *s* without an apostrophe.

       If an acronym already represents a plural noun, do not add an *s*.

       .. note::

          To refer to more than one FAQ document or section, add the
          appropriate noun after *FAQ* and make the noun plural—for example,
          *FAQ articles*. Follow this guideline for other plural acronyms when
          you need to refer to more than one instance of them.

     - CPUs, APIs, IDs, OSs, the 1990s, 0s and 1s

       frequently asked questions (FAQ)
   * - To form the plural of a single letter or a symbol, add an apostrophe and
       a lowercase *s*.
     - x's, #'s
   * - Abbreviated units of measure are both singular and plural; no *s* is
       necessary.
     - 5 mm, 20 in., 20 min
   * - Do not use *(s)*, */s*, *(es)*, or */es* at the end of a word to
       indicate the possibility of more than one item, and do not combine the
       singular and plural forms of a verb, such as *is/are*. Use the singular
       form or the plural form, use both forms joined by a conjunction, or use
       the phrase *one or more*.
     - *Use:*\

       Close any application that is open.

       Close any applications that are open.

       *Do not use:*

       Close any application(s) that is/are open.

Product names and version numbers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

When using Rackspace product names and showing version numbers, observe
the following guidelines:

-  Always spell out and properly capitalize Rackspace product and
   service names (for example, Cloud Servers and Cloud Files).

-  In some cases, you can refer to the product generically after using
   the product name. For example, after you introduce the Cloud
   Monitoring Agent, you can refer to simply *the agent*.

-  Do not capitalize an item that a user creates through a Rackspace
   service. For example, users use the Cloud Servers service to create a
   *server*, not a *Server*, and they use the Cloud Load Balancer
   service to create a *load balancer*, not a *Load Balancer*.

-  Do not abbreviate Rackspace names, unless the abbreviation has been
   approved by the Legal and Marketing departments. For example, never
   abbreviate Cloud Block Storage as CBS.

-  For API documentation, the version number in the documentation should
   match the version number of the software. The combination of the API
   version number and the publication date identify the document
   version.

When using third-party company and product names, use the name as it is
used by the third-party. For a list of commonly used third-party names,
see `Third-party names and
trademarks <../terminology-guidelines.html#third-party-names-and-trademarks>`__.

When referring to an OpenStack service, use the actual service name, and
provide the project name in parentheses. For example, use OpenStack
Block Storage (Cinder). On subsequent references, use the service name
instead of the project name, unless you need to use project names to
differentiate between two versions of one service. See the `OpenStack
documentation
conventions <http://docs.openstack.org/contributor-guide/writing-style/openstack-components.html>`__
for service and project names.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - Use Cloud Servers to create a server.
     - Use Cloud Servers to create a Server.
   * - Use Cloud Block Storage to create volumes.
     - Use CBS to create volumes.
   * - You can add files to a server.
     - You can add Cloud Files to a Cloud Server.
   * - Microsoft SQL Server is supported.
     - MSSQL is supported.
   * - Cloud Servers provides the core features of the OpenStack Compute (Nova)
       API.
     - Cloud Servers provides the core features of OpenStack Nova.


.. _punctuation-guidelines:

Punctuation
~~~~~~~~~~~

Use punctuation correctly and consistently. This section provides
guidelines for using punctuation in Rackspace documentation. For basic
rules about punctuation, see a grammar reference, such as the Harbrace
College Handbook.

-  `Ampersands <#ampersands>`__
-  `Colons <#colons>`__
-  `Commas <#commas>`__
-  `Dashes <#dashes>`__
-  `Ellipses <#ellipses>`__
-  `Exclamation points <#exclamation-points>`__
-  `Hyphens <#hyphens>`__
-  `Parentheses <#parentheses>`__
-  `Periods <#periods>`__
-  `Quotation marks <#quotation-marks>`__
-  `Semicolons <#semicolons>`__
-  `Slashes <#slashes>`__

For general guidelines about using symbols, see `Symbols <#symbols>`__.

Ampersands
----------

Do not use an ampersand (&) in text or headings to mean *and* unless you
are specifically referring to the symbol on the user interface or the
ampersand is part of an official name.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - This article describes the differences between IMAP and POP.
     - This article describes the differences between IMAP & POP.
   * - *(Title)* Setting up Microsoft Exchange 2007 email on your iPhone, iPad,
       and iPod

       *(Title)* Cloud Files: How-to articles and other resources
     - *(Title)* Setting up Microsoft Exchange 2007 email on your iPhone, iPad,
       & iPod

       *(Title)* Cloud Files: How-to articles & other resources
   * - *(Button name includes &)* To continue, click **Save & Go to Step 3**.
     - *(Button name includes &)* To continue, click **Save and Go to Step 3**.
   * - When Peter Medrano, IT Director at Morgan & Sampson, arrived, he found
       employees using disparate, consumer email services from different
       providers.
     - When Peter Medrano, IT Director at Morgan and Sampson, arrived, he found
       employees using disparate, consumer email services from different
       providers.

Colons
------

Use the following guidelines for colons.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - Use a colon at the end of a sentence that introduces a list. If another
       sentence intervenes between the introductory sentence and the list, use a
       period instead of a colon.

       .. note::

          Use a sentence, rather than a fragment, to introduce a list.
          Fragments are difficult to translate and can be harder to comprehend
          than sentences, so avoid using them to introduce lists.
     - The following monitoring checks are available to users:

       You can use this product to perform the following tasks:

       You can use this product to perform the following tasks. You must
       extract objects from the database to complete these tasks.
   * - In steps, use a colon to introduce code that the user is expected to
       enter.
     - Run the following command:

       ``nova list``
   * - In a list item, if you need to separate an initial term or phrase from
       the information that follows it, use a colon.
     - **Public**: This setting allows any two servers with public IP addresses
       to be load balanced. These can be nodes outside of the Rackspace
       network, but if they are, standard bandwidth rates apply.
   * - Do not use a colon to end the introduction to a table, figure, or
       example.
     - The following figure shows an overview of Cloud Databases
       infrastructure.

       In the following request example, ``Content-Type`` is set to
       ``application/json``, but ``application/xml`` is requested in the
       ``Accept`` header.

       Table 5.1 lists the endpoints to use for your Cloud Databases API calls.
   * - Do not use a colon at the end a table column header, a title, or a
       heading.
     - 3.2. Service Endpoints

       To create a monitoring check

       Table 3.1. Regionalized Service Endpoints

       Example 4.4. List Versions Response: JSON

Commas
------

Use the following guidelines for commas. For basic comma usage, see a
grammar reference, such as the *Harbrace College Handbook*.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Guideline
     - Correct
     - Incorrect
   * - In a series of three or more items, use a serial comma (that is, precede
       the conjunction with a comma).
     - You can upgrade, migrate, and integrate the product.
     - You can upgrade, migrate and integrate the product.
   * - Do not use only a comma to separate independent clauses. Doing so
       creates a *comma splice*.

       If you join independent clauses, insert a coordinating conjunction
       between them and precede the conjunction with a comma.
     - Click **Options**, and then click **Allow Fast Saves**.

       The UUID for ServiceNet is ``11111111-1111-1111-1111-111111111111``, and
       the UUID for PublicNet is ``00000000-0000-0000-0000-000000000000``.
     - Click **Options**, then click **Allow Fast Saves**.

       The UUID for ServiceNet is ``11111111-1111-1111-1111-111111111111``, the
       UUID for PublicNet is ``00000000-0000-0000-0000-000000000000``.
   * - Use a comma to set off a nonrestrictive clause (one that begins with
       *which*).

       Do not use a comma to set off a restrictive clause (one that begins with
       *that*).
     - The hourly backups are rolled into a nightly backup, which is retained
       for two days. *(nonrestrictive)*

       Enter the user name and password that you just created. *(restrictive)*
     - The hourly backups are rolled into a nightly backup which is retained
       for two days.

       Enter the user name and password, that you just created.
   * - Use a comma to separate an introductory word, phrase, or clause from the
       rest of the sentence.
     - When you check your email with an IMAP connection, you are accessing and
       managing your email directly from the email server.

       However, you can easily update the version by using the WordPress
       management dashboard.

       Unlike the other alarms in this list, you set the network check alarm
       variable upon network check creation.

       For more information, see Upgrading your Private Cloud.
     - When you check your email with an IMAP connection you are accessing and
       managing your email directly from the email server.

       However you can easily update the version by using the WordPress
       management dashboard.

       Unlike the other alarms in this list you set the network check alarm
       variable upon network check creation.

       For more information see Upgrading your Private Cloud.
   * - Do not use a comma between the verbs in a compound predicate.
     - These open-source Python clients run on Linux or Mac OS X systems and
       are easy to learn and use.
     - These open-source Python clients run on Linux or Mac OS X systems, and
       are easy to learn and use.
   * - When a comma is required after a quotation that is embedded in text,
       place the comma inside the closing quotation mark.
     - In the section called "Parameters," enter the values for length, width,
       and height.
     - In the section called "Parameters", enter the values for length, width,
       and height.
   * - Use commas in numbers with five or more digits. However, do not use
       commas in the following types of numbers: addresses, fractional parts of
       decimal numbers, page numbers, literal representations of user-entered
       values or displayed values

       .. note::

          Do not use European-style numbering, which uses commas in the
          place of periods. For example, use 3.14159, not 3,14159.
     - 9001 N IH 35

       1452.7532

       page 1055

       1024 bytes
     - 9,001 N IH 35

       1,452.753,2

       page 1,055

       1,024 bytes
   * - When city and state names are embedded in a sentence, use a comma after
       the city and the state.
     - The company headquarters were in Kansas City, Missouri, before the
       merger.
     - The company headquarters were in Kansas City, Missouri before the
       merger.
   * - When a month, day, and year are embedded in a sentence, use a comma
       before and after the year. When only the month and year compose the
       date, omit the commas unless the syntax would ordinarily require a comma
       following the year.
     - The company acquired a German subsidiary on July 15, 2009, and is
       negotiating the purchase of a small Japanese company.

       The publications plan was printed in November 2010 in Austin.

       In December 2012, the database restoration failed.
     - The company acquired a German subsidiary on July 15, 2009 and is
       negotiating the purchase of a small Japanese company.

       The publications plan was printed in November, 2010, in Austin.

       In December 2012 the database restoration failed.

.. _dashes:

Dashes
------

An *em dash* is the longest dash. You can use em dashes to set off a
long qualifier in the middle of a sentence if the use of commas would
hinder readability. If you use em dashes for this purpose, do not use
spaces around them.

Don't use an em dash to separate a long sentence into two parts.
Instead, create two sentences.

An *en dash* is longer than a hyphen and shorter than an em dash. Use an
en dash for the following purposes:

-  To show a range of numbers in a table or figure

   .. note::

      To show a range of numbers in text, use *to* or *through* instead
      of an en dash.

-  To represent a minus sign

-  To indicate a negative number

-  To join the elements of a compound modifier when one of the elements
   is an open compound (a combination of words that constitutes a single
   concept, like Customer Support).

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Correct
   * - approximately 10–20 diagrams

       options 11–15

       2010–2013
   * - ``12–13=–1``
   * - Customer Support–related queries

Ellipses
--------

An ellipsis (...) is a punctuation construct that is used in syntax or
to indicate omitted code in technical content. For technical writing, an
ellipsis is used mainly in code examples.

Do not use an ellipsis in the following cases:

-  When writing header text for table columns and rows.
-  When showing the name of an interface element, such as a text box,
   menu, menu command, or command button, even if the ellipsis is
   displayed on the interface. However, if an ellipsis is displayed on
   the interface and you think that omitting it might cause confusion,
   you can include it.

The following example shows acceptable use of an ellipsis in a code
sample:

.. code::

   HTTP/1.1 200 OK
   Content-Location: /v1/queues/fizbat/messages?ids=50b68a50d6f5b8c8a7c62b01,
   f5b8c8a7c62b0150b68a50d6
   ...
   [
   {
   "href": "/v1/queues/fizbit/messages/50b68a50d6f5b8c8a7c62b01",
   "ttl": 800,
   "age": 32,
   "body": {
   "cmd": "EncodeVideo",
   "jobid": 58229
   }
   },

The following examples show when *not* to use ellipses:

On the **File** menu, click **Open...**.

Do this ... *(column header)*

Exclamation points
------------------

Avoid using exclamation points. For more information, see `Use
interjections with
care <../basic-writing-guidelines.html#use-interjections-with-care>`__.

Hyphens
-------

This section provides general guidelines for hyphenation. For guidelines
about using dashes, see `Dashes <#dashes>`__.

-  `Hyphens in compound modifiers <#hyphens-in-compound-modifiers>`__
-  `Hyphens with prefixes <#hyphens-with-prefixes>`__

Hyphens in compound modifiers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When two or more words precede and modify a noun as a unit (also called
a *compound modifier*), use hyphens according to the following
guidelines.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - To clarify meaning, use a hyphen.
     - *Ambiguous:*

       high level language compiler

       (a language compiler that is high level or a compiler of high-level
       languages?)

       *Clear:*

       high-level-language compiler

       (clearly a compiler of high-level languages)
   * - Words that you hyphenate as compound modifiers preceding a noun might
       not be hyphenated in other parts of a sentence or when used as another
       part of speech. Hyphenate only if needed for clarity.

       .. note::

          One exception is *up-to-date*, which is hyphenated in any
          position in a sentence.
     - local-level attributes

       attributes that are defined at the local level

       up-to-date content

       content is up-to-date
   * - If the first component of a compound modifier is a number, use a hyphen.
     - 32-bit operating system

       three-tier architecture

       80-character line length

       3.5-inch disk
   * - If the first word of a compound modifier is an adverb ending in *-ly*,
       do not hyphenate the modifier.
     - newly designed interface

       recently upgraded product

       fully qualified domain name
   * - If one of the elements of a compound modifier is an open compound
       (multiple words that constitute a single concept, like Customer
       Support), use an en dash, not a hyphen, to separate the open compound
       from the rest of the modifier.
     - Customer Support–related queries
   * - If one of the elements of a compound modifier is a trademark, do not
       hyphenate the modifier.
     - *Use:*

       specific to Java

       Java specific

       *Do not use:*

       Java-specific
   * - Avoid using suspended compound adjectives, unless space is limited. In a
       suspended compound adjective, part of the adjective is separated from
       the rest of the adjective, such as *first-* in *first- and
       next-generation servers*. If you must use suspended compound adjectives,
       include a hyphen with both adjectives. Avoid forming suspended compound
       adjectives from one-word adjectives.
     - *Use:*

       You can use any combination of uppercase and lowercase letters in a
       password.

       Click the upper-right or lower-right corner.

       *Avoid:*

       You can use any combination of upper- and lowercase letters in a
       password.

       Click the upper- or lower-right corner.

Hyphens with prefixes
^^^^^^^^^^^^^^^^^^^^^

Words with prefixes are not usually hyphenated. However, a hyphen might
be necessary in the following cases:

-  You need to distinguish between homographs, such as *re-create* and
   *recreate*.

-  The last letter of the prefix and the first letter of the root word
   are the same. Exceptions are words such as *reenter* and
   *preemptive*, which are not likely to be misread.

-  The prefix precedes a proper noun or a number, as in *non-Boolean*
   and *pre-2000*.

-  The product team has hyphenated a term with a prefix, and you need to
   follow suit in the docs for consistency with the interface—for
   example, *multi-factor authentication* in the Identity product.
   Whenever possible, work with the teams to use preferred spelling.

For the correct formatting of a specific word, see a dictionary or
`Terminology <terminology-guidelines.md>`__. For more information about
hyphenating prefixes, see *The Chicago Manual of Style*.

Parentheses
-----------

Avoid parentheses in running text. Parenthetical text can distract the
reader from the main idea of the sentence and disrupt the flow of the
sentence. When possible, put parenthetical information in a separate
sentence.

Following are some acceptable uses for parentheses:

-  To define an abbreviation
-  To show a special character
-  To show an equivalent measurement
-  To show examples
-  To show a concise phrase that qualifies a term, title, or step

Do not add *(s)* or *(es)* to the end of a noun to indicate the
possibility of more than one item. Use the singular form or the plural
form, or use both forms joined by a conjunction.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - An access control list (ACL) allows access from an outside network into
       the ObjectRocket system.

       Object names cannot contain characters such as dollar signs ($) and
       question marks (?).

       One rack unit is 44.45 mm (1.75 in.) high.

       DNS is analogous to a phone book in that it assigns a numerical
       identifier (for example, 210.48.108.35) to a particular name (for
       example, www.diversity.net.nz).

       4. *(Optional)* Enter first and last name information for the mailbox
       owner.

       You can submit up to 10 messages (the default) in a single request.

Periods
-------

Use the following guidelines for periods. For basic period usage, see a
grammar reference, such as the *Harbrace College Handbook*.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - Use a period at the end of a declarative or imperative sentence, and
       insert only one space after the period.
     - I am here. Where are the donuts?
   * - Place periods inside quotation marks, unless the quotation marks are
       part of a literal string. In such cases, place the period outside the
       quotation mark.
     - For more information, see "Trademarks."

       The symbol has one of the following values: ABST, %ABST, or "ABST".
   * - When introducing a list, if one or more sentences separate the
       introductory sentence from the list, end each sentence with a period.
     - You can use this product to perform the following tasks. You must
       extract objects from the database to complete these tasks.
   * - Use periods in list items as follows:

       • If all of the items in a list are sentences, including imperative
         statements, end each item with a period.

       • If all of the items in a list are fragments, do not end the items with
         a period.

       • In a list of fragments, some or all of which are followed by
         sentences, end every fragment and sentence in the list with a period.
     - See the examples in `Writing list items
       <../a-l-style-guidelines.html#writing-list-items>`__.
   * - Use a period after an introduction to a table, figure, or example.
     - The following figure shows an overview of Cloud Databases
       infrastructure.
   * - In glossary definitions, end the definition with a period, even if the
       definition is only a phrase.
     - **token**

       An opaque string that represents an authorization to access cloud
       resources. Tokens might be revoked at any time and are valid for a
       finite duration.
   * - Use periods only with abbreviations that could otherwise be misread as a
       word, such as *in.* (for *inch*). Also, use periods in the abbreviations
       *a.m.* and *p.m.*
     - 25 mm

       12 in.

       FAQ
   * - Precede a file name extension with a period.

       Assume that the period in a file name extension is pronounced as *dot*,
       and use the indefinite article *a*.
     - Copy the **.conf** file to your directory.
   * - Do not end a title or a heading with a period.
     - To create a monitoring check

       Table 3.1. Regionalized service endpoints

Quotation marks
---------------

Refer to quotation marks as *quotation marks*, not as *quote marks* or
*quotes*.

Use single and double quotation marks according to the following
guidelines.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - Use quotation marks in user entries or syntax only if the software
       requires the quotation marks.
     - Replace the text inside of the quotation marks on the ``AuthName`` line
       to the name of your password protected area. For example, type ``"My
       Password Protected Directory"``.
   * - Use quotation marks in message text only if the product shows quotation
       marks in the generated message. Use code font (monospace) to format
       messages.
     - The message ``Press "Enter" to continue`` is displayed in the
       lower-right corner.
   * - If you use a term in a unique or qualified sense, use double quotation
       marks in text only at its first occurrence, and omit the quotation marks
       in subsequent occurrences of the term.
     - The spelling checker "learns" the word. After it learns the word, the
       spelling checker ignores subsequent occurrences of the word in the
       document.
   * - When referring to a section of a web page, enclose the section title in
       parentheses if you cannot create a link.
     - For information about patents, see the "Resources and Tools" section of
       the `Racklaw website <https://inside.rackspace.com/web/racklaw/ip>`__.
   * - Include appropriate punctuation, such as periods and commas, inside
       quotation marks unless the quotation marks are part of the syntax that
       the user must type.

       For more information about using quotation marks with other marks of
       punctuation, see *The Chicago Manual of Style*.
     - For more information, see "Trademarks."

       The symbol has one of the following values: ABST, %ABST, or "ABST".
   * - Do not use quotation marks for emphasis. Use italics instead.
     - Do not use quotation marks for emphasis.
   * - Use quotation marks to enclose text that is used verbatim from another
       source, or to enclose quotations from people.
     - "None did as good a job as Rackspace for experience and spam detection,"
       Woods said.

Semicolons
----------

Avoid using semicolons, which are often misused and even when used
correctly can make sentences longer and more difficult to understand.

- Instead of connecting independent clauses with a semicolon, break them into
  separate sentences.
- Instead of connecting more than two items with semicolons, create a list.

Slashes
-------

Do not use a slash mark (/) to present a choice among, or a series of,
actions or objects. Rewrite the phrase to eliminate the slash mark.
Exceptions are established terms like *client/server* and *read/write*.

Do not use a slash in dates. For information about how to format dates,
see `Dates <../a-l-style-guidelines.html#dates>`__.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Correct
     - Incorrect
   * - You can choose Cloud Backups, Cloud Files, or both.
     - You can choose Cloud Backups and/or Cloud Files.
       You can choose Cloud Backups/Files.
   * - To access your computer, plug it in, log in to the operating system, and
       type your password.
     - To access your computer, plug in the computer/log on/type your password.

Symbols
~~~~~~~

Symbols are used in code, as punctuation, with numbers, and to indicate
trademarks. Use the following general guidelines when you include
symbols in your documentation.

For guidelines about using specific marks of punctuation, see
`Punctuation <#punctuation>`__.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - When referring explicitly to a symbol in text, do not show only the
       symbol. Show the name of the symbol, or the name followed by the symbol
       in parentheses.

       On subsequent uses of the symbol, you can use just the name.

       If the symbol is a common mark of punctuation, like a period or a comma,
       do not show the mark in parentheses.
     - Escape the line by typing a backslash (/) character.

       To find files that were modified more than two days ago, type a plus
       sign (+) in front of the 2.

       Type a comma.
   * - Use a symbol *instead of* the name of the symbol only if space is
       limited (for example, in a table). Do not use symbols in running text.
     - *Body text:*

       45 percent

       16 degrees

       1,800 dollars

       *Limited space:*

       45%

       16º

       $1,800
   * - Do not insert a space between a number and a symbol, except when the
       symbol is used as a mathematical operator.
     - For files that use a total of 1,500 KB and a record size of 256, the
       equation is as follows: ``1,500,000 ÷ 256 = 5,860``
   * - To separate the options in a menu path, use right-angle brackets (>)
       surrounded by spaces.
     - Open Mac Mail and select **Preferences > Accounts**.

Tables
~~~~~~

Often text that is difficult to read in paragraph form is clear when put
into a table. Tables clarify the relationships among information, and
they are easy to scan. This topic provides the guidelines for the
following aspects of tables:

-  `Introductory text for tables <#introductory-text-for-tables>`__
-  `Table titles (captions) <#table-titles-captions>`__
-  `Column and row headers <#column-and-row-headers>`__
-  `Table text <#table-text>`__
-  `Table footnotes <#table-footnotes>`__
-  `Attribute or parameter tables in API
   documents <#attribute-or-parameter-tables-in-API-documents>`__

Table examples are presented in a separate section at the end of this
topic.

.. note::

   Do not create tables that are overly complex or that scroll
   horizontally. If you find that you have too much information in a table,
   try to break it up into smaller tables.

Introductory text for tables
----------------------------

In the text that precedes a table, introduce the table in a way that
relates the table to the text. If the table immediately follows the
reference to it, use a generic reference (such as *the following table*)
even if the table has a title. Provide a link to a table title only when
the table does not immediately follow the reference or when the table is
in a different article or section.

To introduce a table, use a sentence (not a fragment), and end it in a
period (not a colon).

Table titles (captions)
-----------------------

Tables should normally have titles (captions). However, some tables are
closely associated with the surrounding text and do not require titles.
For example, decision matrixes and tables within tasks, procedures, and
tutorials do not require numbers or titles.

When creating table titles, use the following guidelines:

- Use sentence-style capitalization for table titles. However, for words that
  are always uppercase or always lowercase, match that case.
- Do not start a table title with an article (*a*, *an*, *the*).
- Do not end a table title with a period or colon.
- Place the title above the table, not below it, and tag it as bold.
- Do not manually number table titles. If titles should be numbered, the style
  sheet will number them.
- Make table titles concise; limit them to one line if possible.
- Make table titles descriptive:

  - Avoid using a table title that duplicates a topic or section title.
  - Ensure that no two table titles in an article are identical. To distinguish
    between the titles that are similar, add qualifiers.

- Do not include trademark symbols in table titles.

Column headers
--------------

Use the following guidelines for text in column headers:

-  Use `sentence-style
   capitalization <../a-l-style-guidelines.html#cap-sentence-style>`__
   in column headers. However, for words that are always uppercase or
   always lowercase, match that case.
-  Use singular nouns for column headers, unless the context requires
   otherwise.
-  Do not end column headers with ellipses or colons.

Table text
----------

Use the following guidelines for text in table cells:

-  Use the same punctuation and capitalization guidelines that you use
   for `text in lists <../a-l-style-guidelines.html#lists>`__.
-  Make the entries in a table parallel. For example, in a column that
   describes options, be consistent in beginning the entries with a verb
   or noun.
-  Avoid leaving a table cell blank. If no information is available for
   that cell, use *Not applicable* or *None*. Use the abbreviation *NA*
   only if space constraints exist. Do not use dashes. An exception is
   for matrix-type tables that use an X or other marker to indicate
   support. In such cases, blank cells are acceptable (see the third
   example in the sidebar).
-  When showing a notation in a table, use the guidelines in `Notes and
   other notation types <#notes-and-other-notation-types>`__.
-  If space in a table is constrained, you can use abbreviations and
   symbols that you would not normally use in body text (such as % for
   percent).
-  Do not use color to differentiate table text.

Table footnotes
---------------

If a notation (for example, a note or warning) applies to the entire
table, place the content in a regular notation preceding the table. If a
notation applies only to the content in a certain cell, place the
notation in that cell. However, if a notation applies to all of the
content in a row or column, or to the content in two or more cells, you
can use footnotes.

-  When writing the text of table footnotes, use the following
   guidelines:

   -  Ensure that all footnotes are written clearly and completely. Use
      sentences when possible. Avoid cryptic language.
   -  Ensure that all footnotes have parallel grammatical structure
      (sentences are paralleled by sentences, phrases by phrases, and so
      on).

-  Place the footnote text at the end of the table, either in a final
   row that spans the entire table or under the last row in the table.

-  Use superscript numbers to indicate the footnotes in the cells to
   which they apply. If numbers might be confusing (for example, because
   the text in the cells are numerical values), use lowercase letters
   instead.

   -  A footnote cited in a column header applies to the entire column.
   -  A footnote cited in a table cell applies to the text in that cell.
      Use a cell-level footnote if the note applies to multiple cells in
      the table.

Attribute or parameter tables in API documents
----------------------------------------------

When creating attribute or parameter tables in API documents, use the
following additional guidelines:

-  For tables that describes JSON or XML attributes, write the first
   sentence of a description with an implied subject. For example, if
   the attribute is name, the description might be as follows: "Server
   name, which becomes the initial host name of the server"
-  For attributes, include the valid values and default value at the end
   of the description. Use the formats "Valid values are *n* and *n*."
   and "The default is *n*." For example, "Valid values are ``true`` and
   ``false``." and "The default is ``false``."
-  If table descriptions or construction is complex, consider using a
   definition list or itemized list instead of a table.
-  Avoid putting definition lists in tables.

Examples
--------

The different parts of the preceding URL are explained in the following
table.

.. list-table::
   :widths: 30 70
   :header-rows: 1

   * - Part of URL
     - Explanation
   * - ``swift://``
     - The prefix that passes file system requests to the Swift file system.
   * - ``acontainer``
     - The name of the container in Swift that contains the objects to be
       accessed. Container names must conform to RFC952 restrictions for host
       names—that is, the characters A-Z, numbers 0-9, and the hyphen (-).

       Nonconforming container names are inaccessible by swiftfs.
   * - ``aservice``
     - A user-friendly "service" name. A service name maps to a collection of
       configuration entries in the Hadoop core-site.xml file that specify
       where the container is located (for example, rackspace-dfw).
   * - ``/path/to/files``
     - The name of the object or objects in Swift to be referenced. Although
       Swift doesn't support paths, swiftfs attempts to interpret names that
       look like paths and behave appropriately. For example, an input path
       named ``/path/to/*`` would qualify all objects with names prefixed by
       ``/path/to/``. Similarly, an output path of ``/path/to/`` would prefix
       the names of all newly created objects with ``/path/to/``.

The following table provides the default values for the absolute limits.

**Absolute limits**

.. list-table::
   :widths: 25 50 25
   :header-rows: 1

   * - Name
     - Description
     - Limit (default value)
   * - Node count
     - Maximum number of allowed data nodes
     - 3
   * - Disk
     - Maximum disk capacity across all data nodes, in gigabytes (GB)
     - 4500
   * - RAM
     - Maximum RAM across all data nodes, in gigabytes (GB)
     - 23040
   * - VCPUs
     - Maximum virtual CPUs across all data nodes
     - 6

The following matrix indicates which upgrade scenarios are supported.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Upgrade scenario
     - Supported
     - Not supported
   * - 4.2.0 to 4.2.\ *x*
     -
     - X
   * - 4.1.\ *x* to 4.2.1
     - X
     -
   * - 4.1.\ *x* to 4.2.0
     -
     - X
   * - 4.1.\ *x* to 4.1.\ *x*
     - X
     -
   * - 4.0.0 to 4.2.\ *x*
     -
     - X
   * - 4.0.0 to 4.1.\ *x*
     - X
     -
   * - 3 (OpenCenter) to any version
     -
     - X
   * - 2 (Alamo) to any version
     -
     - X

The following chart compares these top content management systems
(CMSs).

.. list-table::
   :widths: 20 40 40
   :header-rows: 1

   * -
     - Drupal
     - WordPress
   * - **Homepage**
     - www.drupal.org
     - www.wordpress.org
   * - **About**
     - Drupal is a powerful, developer-friendly tool for building complex
       sites. Like most powerful tools, it requires some expertise and
       experience to operate.
     - WordPress began as an innovative, easy-to-use blogging platform. With an
       ever-increasing repertoire of themes, plug-ins, and widgets, this CMS is
       also widely used for other website formats.
   * - **Example sites**
     - Community Portal: Fast Company, Team Sugar
     - Social Networking: PlayStation Blog

       News Publishing: CNN Political Ticker

       Education/Research: NASA Ames Research Center

       News Publishing:The New York Observer
   * - **Installation**
     - Drupal Installation Forum
     - WordPress Installation Forum

Tasks and procedures
~~~~~~~~~~~~~~~~~~~~

A *task* is a job that customers perform to achieve a goal, such as
creating a server. A task is made up of a number of elements, including
procedures, which are sets of sequential action steps. A task topic,
article, or section focuses on the customer’s task. It provides the
action steps and the essential supporting information (context and
reference) that the customer needs to complete the task.

This topic provides guidelines for developing task topics and
procedures.

-  `Task titles <#tasks-titles>`__
-  `Task introductions <#task-introductions>`__
-  `Prerequisites <#prerequisites>`__
-  `Procedural steps <#procedural-steps>`__
-  `Results, verification, examples, and
   troubleshooting <#results-verification-examples-and-troubleshooting>`__
-  `Direction to the next action <#direction-to-the-next-action>`__
-  `Related topics <#related-topics>`__

Task titles
-----------

The title of a task topic, article, or section begins with the
imperative form of the task action and uniquely, precisely, and clearly
describes the task. Use a plural subject unless the singular makes more
sense or is necessary for clarity.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - Create users in SQL Server

       Configure SQL Server Management Studio to connect to SQL Server on
       Windows

       Add new ServiceNet routes to a server
     - Creating users in SQL Server

       How to create users in SQL Server

       To create users in SQL Server

For guidelines about capitalizing titles, see
`Capitalization <../a-l-style-guidelines.html#capitalization>`__.

Task introductions
------------------

Before providing steps, set the context for the task as necessary. For
example, briefly state the reason for completing the task, the method to
be used, and the expected result. You might also suggest the amount of
time that the task should take, especially if it will take a long time.

A simple task might require only one or two sentences of introduction
and a single set of steps. However, a complex task might require several
procedures and even reference material. In the latter case, you can
include the following kinds of information in the introduction:

-  High-level description of the associated tasks and their
   relationships, including a forecast of the upcoming actions
-  Common requirements for the tasks
-  High-level sequence of events
-  Flow chart
-  Hyperlinks to material that the customer needs to review
-  Knowledge requirements for customers

**Notes:**

- If the article or section title provides sufficient context, you
  can omit an introduction.
- Avoid providing extensive overview or conceptual text in the
  introduction to a task. Provide that information in a separate
  concept topic or in a topic that introduces the task as part of
  a larger process or customer goal.

Prerequisites
-------------

If the task has requirements that the customer *must* meet before taking
action, describe these in a "Prerequisites" section that precedes the
procedure. You might include the following information:

-  A hyperlink to a preceding task, if that task must be performed
   before this task
-  Software that must already be installed, accessible, or running
-  Access rights that are required for customers to perform the task
-  Hyperlinks to other topics that contain requirements or prerequisite
   tasks that the customer must perform

.. note::

   Avoid including detailed procedures in a prerequisites
   section. Provide prerequisite tasks in other articles or sections, which
   you can reference in this section.

Procedural steps
----------------

A task contains one or more procedures, or sets of sequential action
steps. Consider the following guidelines when creating a procedure:

-  If the procedure has more than one step, use a numbered list for the
   steps. Do not use bullets, except to list choices within a step.
-  If the procedure has only one step, show that step in a regular
   paragraph. That is, do not number it.
-  If you have lengthy introductory or prerequisite information, or if
   you have more than one procedure, provide a heading for the procedure
   or procedures. Use the imperative form of the action and a singular
   form of the object. Do not repeat the title of the task article.
-  Try to limit procedures to 10 steps. If you have more than 10 steps,
   consider whether you can divide the steps into two or more
   procedures. Creating several short, simple, and sequential procedures
   instead on one long, complex procedure, especially one with many
   substeps and choice steps, will help customers know where they are in
   the process, judge their progress, and complete the task
   successfully.

When writing steps, use the following guidelines.

-  `Use imperative sentences <#use-imperative-sentences>`__
-  `Show one action per step <#show-one-action-per-step>`__
-  `Use consistent verbs <#use-consistent-verbs>`__
-  `Provide context before the
   action <#provide-context-before-the-action>`__
-  `Provide conditions before
   actions <#provide-conditions-before-actions>`__
-  `Follow the step with explanatory
   information <#follow-the-step-with-explanatory-information>`__
-  `Show only actions as steps <#show-only-actions-as-steps>`__
-  `Use screenshots sparingly <#use-screenshots-sparingly>`__
-  `Label optional steps <#label-optional-steps>`__
-  `Omit extraneous words <#omit-extraneous-words>`__
-  `Show multiple conditions in a
   list <#show-multiple-conditions-in-a-list>`__
-  `Show multiple possibilities in a
   list <#show-multiple-possibilities-in-a-list>`__
-  `Document only one method <#document-only-one-method>`__

Use imperative sentences
^^^^^^^^^^^^^^^^^^^^^^^^

Write each step as a complete and correctly punctuated imperative
sentence (that is, a sentence that starts with an imperative verb). In
steps, the `focus <../basic-writing-guidelines.html#write-to-user>`__ is
on the customer, and the
`voice <../basic-writing-guidelines.html#use-active-voice>`__ is active.

**Examples**

#. Log in to the Cloud Control Panel.

#. Use the following command to start ``vsftpd``:

   .. code::

      sudo service vsftpd start

Show one action per step
^^^^^^^^^^^^^^^^^^^^^^^^

Usually, include only a single action in each step. If two actions are
closely related, such as opening a menu and selecting a command from the
menu, you can include both actions in one step.

**Examples**

*Use:*

#. Under **Export**, select your database (for example, 388488\_drupal).

#. Scroll down to the bottom of the window and select the **Save as
   file** check box, which will save your database output to a file.

#. Click **Go**.

#. If you are prompted to save your file, save it to your computer.

*Do not use:*

Under **Export**, select your database (for example, 388488\_drupal).
Scroll down to the bottom of the window and select the **Save as file**
check box, which will save your database output to a file. Finally click
**Go**. If you are prompted to save your file, save it somewhere on your
computer.

Use consistent verbs
^^^^^^^^^^^^^^^^^^^^

Use the following action verbs consistently:

- *Click*, to refer to command buttons, hyperlinks, icons, and tabs
- *Select*, to refer to items that the customer can select from a list,
  option buttons, menu commands, and menu sequences
- *Select* and *clear*, to refer to check boxes

**Example**

#. On the Binding and SSL Settings page, perform the following steps:
#. Select an IP address, or select the default value of **All Unassigned**.
#. Select the **Start FTP site automatically** check box.
#. Select **Allow SSL**.
#. Click **Next**.

Provide context before the action
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If a step specifies where to perform an action, state where to perform
the action before describing the action.

**Examples**

#. In the navigation pane, click **Inbound Rules**.

#. On the Binding and SSL Settings page, perform the following steps:

Provide conditions before actions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If a step specifies a situation or a condition, state the situation or
condition before describing the action.

**Examples**

#. If a new version is available, click **Install**.

#. To find out the encryption type of your Windows computer (32-bit or
   64-bit), navigate to the server's Control Panel and click **System**.

Follow the step with explanatory information
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Do not include explanatory or reference information in the action part
of a step. If needed, follow the step with one or more paragraphs that
provide supplemental information.

**Examples**

#. In the **Body Match** text box, enter a word or phrase that will
   appear on the page when it loads successfully.

   For example, you can perform a body match on the copyright date to
   verify whether the website is running.

Show only actions as steps
^^^^^^^^^^^^^^^^^^^^^^^^^^

Do not document system actions, responses, or results as steps. Put
necessary statements in paragraphs following the steps to which they
apply. See the first *Use/Do not use* example in the "Examples" section.

When the result of a step is the appearance of a dialog box, window, or
page in which the action of the next steps occurs, you can usually
eliminate a result statement and orient the customer at the beginning of
the next step. See the second *Use/Do not use* example in the "Examples"
section. However, include results statements when the results are not
obvious or you think that customers need a checkpoint in a procedure.

**Examples**

*Use:*

#. On Linux, enter the following command:

   .. code::

      sudo rackspace-monitoring-agent --setup

   The list of setup settings is displayed.

*Do not use:*

#. On Linux, enter the following command:

   .. code::

      sudo rackspace-monitoring-agent --setup

#. The list of setup settings is displayed.

*Use:*

#. Under **Other Options** in the Rackspace Email box, select **Mobile
   Sync**.
#. On the Activate Mobile Sync page, select individual users to
   activate, or select the **Add Mobile Sync to all mailboxes on this
   domain** option.

*Avoid:*

#. Under **Other Options** in the Rackspace Email box, select **Mobile
   Sync**.

#. The Activate Mobile Sync page is displayed.

#. Select individual users to activate, or select the **Add Mobile Sync
   to all mailboxes on this domain** option.

Use screenshots sparingly
^^^^^^^^^^^^^^^^^^^^^^^^^

Screenshots can help to orient the customer, but a screenshot of every
field or dialog box is usually not necessary.

If you include screenshots, place each one directly under the step that
it illustrates. Do not rely on the screenshot to show information or
values that the user must enter; always provide that information in the
text of the steps. However, ensure that the screenshot accurately
reflects the directions and values in the step text.

Label optional steps
^^^^^^^^^^^^^^^^^^^^

To indicate that a step is optional, include *(Optional)*, in italics,
as a qualifier at the beginning of the step.

**Example**

#. *(Optional)* Click **Advanced Options**.

Omit extraneous words
^^^^^^^^^^^^^^^^^^^^^

Omit extraneous words (such as *pop-up menu* or *command button*) unless
the omission sacrifices clarity.

**Examples**

*Use:*

#. In the Disks window, right-click the volume and select **Take
   Offline**.

*Avoid:*

#. In the Disks window, right-click the volume and select **Take
   Offline** from the pop-up menu.

*Use:*

#. Click **Add**, enter a name for the profile, and then click **OK**.

*Avoid:*

#. Click the **Add** button, enter a name for the profile in the text
   box, and then click the **OK** button.

Show multiple conditions in a list
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If the action of a step varies depending on multiple conditions, use an
unordered list to present the conditions.

**Example**

#. At the next prompt, associate one of the listed Cloud Monitoring
   entities with the agent:

   -  If only one entity is listed, select option 1.
   -  If more than one entity is listed, choose the entity that most
      closely matches your server based on the IP addresses listed.

Show multiple possibilities in a list
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If a step directs the customer to choose from multiple possibilities,
use an unordered list to present the possibilities.

**Example**

#. Select a volume type:

   -  **Standard**: A standard SATA drive for customers who need additional
      storage on their server
   -  **High Performance**: An SSD drive, which offers a higher performance
      option for databases and high performance applications

Document only one method
^^^^^^^^^^^^^^^^^^^^^^^^

If more than one method exists for completing an action, document only
one method, usually the most efficient or preferred method.

**Example**

*Use:*

#. Select **File > New**.

*Do not use:*

#. Select **File > New**, or press **Ctrl+N**.

Results, verification, examples, and troubleshooting
----------------------------------------------------

Following the procedure or procedures, include the following information
if it is necessary or helpful to the customer. If the information is
brief, you can include it directly following the last step in the
procedure. If it is lengthy or you need to provide more than one type of
information, use sections with headings.

-  The result of performing the task.
-  Information about verifying successful completion of the task, such
   as the location of logs. If verification is a separate task in a
   different article or section, provide a hyperlink to it under a
   "Where to go from here" heading.
-  An example that illustrates or supports the task.
-  Information about what to do if the procedure does not work. This
   information might be a hyperlink to a troubleshooting topic.

Direction to the next action
----------------------------

If your task is part of a larger set of tasks, you can help the customer
by including a "Where to go from here" section. You might include the
following information:

-  A brief explanation of the next task and why the customer needs to
   perform it, accompanied by a hyperlink to the next task.
-  Hyperlinks to other tasks that could be done next, if multiple
   options are available. Describe the multiple options so that
   customers know which task to choose.

Related topics
--------------

To provide a quick way for the customer to access other content that is
related to the task, provide links to the content at the end of the
article or topic. Even if you have already included an embedded
hyperlink to the material in the article or topic, you can provide the
hyperlink again under "Related topics," but typically you should provide
a link only once in an article or section. For more information about
linking, see `Links and
cross-references <../a-l-style-guidelines.html#links-and-cross-references>`__.

Telephone numbers
~~~~~~~~~~~~~~~~~

Use the following guidelines for telephone numbers:

Use a space, not hyphens or dashes, to separate parts of the telephone
number.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - 1 210 312 4600
     - 1-210-312-4600
   * - 1 800 961 4454
     - 1 (800) 961-4454

Precede US and Canadian telephone numbers with 1. Precede all other
telephone numbers with a plus sign.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - US and Canadian
     - All others
   * - 1 210 312 4600
     - +44 0 20 8734 2700

       +45 7734 5764

If you are showing phone numbers in screenshots or in examples, use the
following guidelines:

-  Do not use any number that might be a real telephone number. Instead,
   use a number in the range 555-0100 through 555-0199; these numbers
   are reserved for fictional use. You can also use a number that
   belongs to Rackspace.
-  If a screenshot includes a nonfictional, non Rackspace number, mask
   out all or parts of it.

Text formatting
~~~~~~~~~~~~~~~

Certain text should be formatted differently from the surrounding text
to designate a special meaning or to make the text stand out to the
customer. Usually this formatting is accomplished by applying a
different font treatment (bold, italics, or monospace).

.. note::

   *Monospace* is also called a *fixed-pitch* or *fixed-width*
   font. In monospace, each letter and character occupy the same amount of
   horizontal space. An example of a monospace font is Courier, and it
   looks as follows: ``monospace font``.

Observe the following general guidelines when formatting text:

-  To apply a font treatment, use the appropriate markup in your
   authoring tool. In RST, use a directive if one is available. See the
   tables in this section for details.

   .. note::

      Apply directives only if the style sheet has been updated to
      support them. If they are not supported, apply formatting manually.

-  Do not apply font treatments to text elements in titles and headings.
-  Do not use capitalization to emphasize a term (for example, showing a
   general term in all capitals). Follow the capitalization that is
   normally used for a term, or follow the capitalization guidelines in
   the following table. For more information, see
   `Capitalization <../a-l-style-guidelines.html#capitalization>`__.
-  Do not use color alone to distinguish text. Color is powerful but
   unreliable. Not everyone can see every color, most people do not
   print using color, and monitors and browsers limit themselves to
   color subsets. Also, people can personalize their displays to
   override your color selections.
-  Use quotation marks only as directed in this topic and in `Quotation
   marks <#quotation-marks>`__.

The conventions are divided into tables based on the content in which
they would most likely be used. If you can't find what you are looking
for in one table, be sure to look in the others.

-  `Conventions for common items <#conventions-for-common-items>`__
-  `Conventions for API and CLI <#conventions-for-api-and-cli>`__
-  `Conventions for UI <#conventions-for-ui>`__

.. note::

   Any differences in style between Public Cloud and Private
   Cloud are highlighted.

Conventions for common items
----------------------------

The following table lists formatting conventions for items that might
appear in content that documents a UI, CLI, or API.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Text item
     - Treatment
     - Output example
   * - Application names
     - Regular text
     - You must configure the RabbitMQ application.
   * - Book titles
     - Italic

       .. note::

          Use italic even if the title is a hyperlink.

     - For the most up-to-date information about rate and absolute limits, see
       the Limits section in the *Rackspace Cloud Databases Developer Guide*.
   * - Cross-references
     - See `Links and cross-references
       <../a-l-style-guidelines.html#links-and-cross-references>`__.
     - Not applicable
   * - Document titles
     - Italic

       .. note::

          Use italic even if the title is a hyperlink.

     - For the most up-to-date information about rate and absolute limits, see
       the Limits section in the *Rackspace Cloud Databases Developer Guide*.
   * - Email addresses
     - See `Email addresses <../a-l-style-guidelines.html#email-addresses>`__.
     - Not applicable
   * - Emphasis
     - Italic
     - Offset *must* be a multiple of the limit (or zero); otherwise, a Bad
       Request exception is generated.
   * - Equations
     - Monospace
     - ``(600,000 – 400,000) ÷ 400,000 = 50%``
   * - Error messages
     - Monospace
     - In SQL Server Management Studio, when you right-click a SQL Server 2012
       database and selecting **Properties**, the following error message
       appears:

       .. code::

          The user does not have permission to perform this action.

   * - Hyperlinks (live)
     - See `Links and cross-references <a-l-style-guidelines.md#links>`__.
     - Not applicable
   * - Keyboard key combinations, names, and shortcuts
     - *(Public)* Bold

       *(Private)* Monospace
     - *(Public)* To skip to the end of the file, press **Shift-G**.

       *(Public)* Press **Enter**.

       *(Private)* To skip to the end of the file, press ``Shift-G``.

       *(Private)* Press ``Enter``.
   * - Letters as letters
     - Italic
     - Place *i* before *e* except after *c*.
   * - Links (live)
     - See `Links and cross-references
       <../a-l-style-guidelines.html#links-and-cross-references>`__.
     - Not applicable
   * - Messages, error
     - Monospace
     - In SQL Server Management Studio, when you right-click a SQL Server 2012
       database and selecting **Properties**, the following error message
       appears:

       .. code::

          The user does not have permission to perform this action.

   * - New terms
     - Italic
     - Cloud Servers that are built using the base Linux images are created
       without a dedicated swap partition and with *swappiness* (a measure of
       how the Linux kernel tries to use swap memory) set to 0.
   * - Permissions
     - Regular text
     - Log in to a shell as the user who has write permissions to
       ``/usr/local/bin`` on your local computer.
   * - Placeholder text (variable text)
     - See `Placeholder (variable) text <#placeholder-variable-text>`__
     - Not applicable
   * - Privileges
     - Regular text
     - The following examples assume that you are making the firewall changes
       as a normal user with sudo privileges.

       The user is granted ALL privileges on the database.
   * - Qualifiers
     - Italic
     - 1. *(Optional)* Enter a new name for the image.

       You can tell that the Managed Cloud post-build automation has
       successfully completed as follows:

       *(Windows servers)* The following file is created:
       **C:\\windows\\temp\\rs\_managed\_cloud\_automation\_complete.txt**

       *(Linux servers)* The following file is created:
       **/tmp/rs\_managed\_cloud\_automation\_complete**
   * - Quotations

       (content quoted from another source)
     - Quotation marks, or block quote formatting
     - "Scalability is key for our business," explained Nathan Goff, Inavero
       Operations Director and Partner. "There's nothing worse than making our
       clients look bad to their customers."
   * - Role names
     - Regular text
     - The full access role has the permissions to create, read, update, and
       delete resources within multiple designated products where access is
       granted.
   * - Terms, new
     - Italic
     - Cloud Servers that are built using the base Linux images are created
       without a dedicated swap partition and with *swappiness* (a measure of
       how the Linux kernel tries to use swap memory) set to 0.
   * - Terms, unique sense
     - Regular text

       Quotation marks on first use
     - The spelling checker "learns" the word. After it learns the word, the
       spelling checker ignores subsequent occurrences of the word in the
       document.
   * - URLs (not live)
     - Bold
     - To access the web interface, open your web browser and navigate to
       **http:// *yourDomain.com*/zipit-install.php**.
   * - URLs (live)
     - See `Links and cross-references
       <(../a-l-style-guidelines.html#links-and-cross-references)>`__.
     - Not applicable
   * - Variable text (placeholder text)
     - See `Placeholder (variable) text <#placeholder-variable-text>`__
     - Not applicable
   * - Words as words
     - Italic
     - Do not use *button* and *icon* interchangeably. If you are referring to
       a command button or toolbar button (labeled or unlabeled), use *button*.
       If you are referring to a graphic on a screen, window, or other area,
       use *icon*.

Conventions for API and CLI
---------------------------

The following table lists formatting conventions for items that usually
appear in content that documents a CLI or API environment.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Text item
     - Treatment
     - Output example
   * - API operation names
     - Regular text

       All lowercase
     - The following table describes the request attributes for the operation
       for migrating vaults.
   * - Argument names
     - Monospace
     - To list or retrieve files from a node that is running the OpenCenter
       agent, use the ``file`` argument with the ``opencentercli`` node
       command.
   * - Attribute names
     - Monospace
     - The ``expires`` attribute denotes the time after which the token
       automatically becomes invalid.
   * - Code
     - Monospace
     - ``$ grep "ftp" /etc/xinetd.d/*`` ``/etc/xinetd.d/vsftpd:service ftp``
       ``/etc/xinetd.d/vsftpd:server = /usr/sbin/vsftpd``

       To set the environment variable, run ``export token="token"``.
   * - Command names (CLI)
     - *(Public)* Monospace

       *(Private)* Bold, by applying the ``:command:`` directive in RST
     - *(Public)* You can check the architecture on Linux by using the ``uname
       -a`` command.

       *(Private)* You can check the architecture on Linux by using the **uname
       -a** command.
   * - Command syntax
     - Monospace
     - If a service is not running, use the service command to start it, as
       follows:

       ``$ sudo service httpd start``
   * - Database names
     - Monospace
     - Start by creating a new database called ``mytestdb``.
   * - Directory names
     - Monospace
     - The following example shows a basic configuration for the FTP service,
       in a file in the ``/etc/xinetd.d directory``.
   * - Element names
     - Monospace
     - The ``message`` element returns a human-readable message that is
       appropriate for display to the end user.
   * - Environment variables
     - Monospace
     - You can set the ``MYSQL_HOST`` environment variable to the remote host's
       address.

       You can export the tenant ID to the ``$account`` environment variable
       and the authentication token to the ``$token`` environment variable.
   * - Examples, code
     - Monospace
     - ``$ grep "ftp" /etc/xinetd.d/*`` ``/etc/xinetd.d/vsftpd:service ftp``
       ``/etc/xinetd.d/vsftpd:server = /usr/sbin/vsftpd``
   * - File names and extensions
     - Monospace
     - To remove the ``vs_quantum-api.cfg`` file from the ``haproxy.d``
       directory and retain it, you can move it to another directory.
   * - Flags
     - Monospace
     - Use the ``-t`` flag to add a time stamp to the results.
   * - Folder names
     - Monospace
     - Copy the ``index.php`` file from your computer to the ``content``
       folder.
   * - Functions
     - Monospace
     - Container names are sorted based on a binary comparison, a single
       built-in collating sequence that compares string data using the
       ``memcmp()`` function, regardless of text encoding.
   * - HTML tags
     - Monospace
     - Avoid putting the ``xml:id`` attribute on the ``title`` tag.
   * - Method names (HTTP)
     - Bold

       All capitals
     - Client authentication is provided through a REST interface by using the
       **GET** method.
   * - Option names, command
     - Monospace

       In RST, apply the ``:option:`` directive.
     - The ``--ip-addresses`` option specifies the IP address and an alias for
       the target.
   * - Package names
     - Monospace
     - You must install the ``libvirt`` package.
   * - Parameter names
     - Monospace

       In RST, apply the ``:option:`` directive.
     - The ``display_description`` parameter is optional.

       Use the ``--flavor`` and ``--image`` parameters to specify the IDs or
       names of the flavor and image to use for the image.
   * - Paths
     - Monospace
     - The path to Perl is ``#!/usr/bin/perl -w``.

       In the URI path ``https://incident.api.rackspacecloud.com/v1/...``, the
       API version is 1.
   * - Syntax statements
     - Monospace
     - The main command used to change a file’s owner or group is ``chown``.
       The most common syntax used with ``chown`` is as follows:

       ``chown user:group file1 file2 file3``
   * - User input
     - Monospace
     - Create a file by using a text editor, and insert the following code:
       ``<?php phpinfo(); ?>``

       For the username, enter ``admin``.
   * - Variables, environment
     - Monospace
     - You can set the ``MYSQL_HOST`` environment variable to the remote host's
       address.

       You can export the tenant ID to the ``$account`` environment variable
       and the authentication token to the ``$token`` environment variable.

Conventions for UI
------------------

The following table lists formatting conventions for items that usually
appear in content that documents a graphical UI.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Text item
     - Treatment
     - Output example
   * - Area (group box) names
     - Bold
     - In the **Edit Signature** area, enter the text that you want to appear
       in your signature.
   * - Box names
       (check box, combo box, group box, list box, spin box, text box, but not
       dialog box)
     - Bold
     - Select the **Manually configure server settings or additional server
       types** check box.

       Retype the password that you entered in the **Password** box.
   * - Button names
       (command, option, radio)
     - Bold
     - Select **Microsoft Exchange** and then click **Next**.
   * - Cascades
       (menu, field)
     - Bold

       Use **>** to separate.

       In RST, apply the ``:menuselection:`` directive.
     - Select **Start > Control Panel**, and then click the **Mail** icon.

       You can find more documentation about RackConnect in the **Community >
       Discussions > RackConnect** section of the MyRackspace Portal.
   * - Check box names
     - Bold
     - Select the **Manually configure server settings or additional server
       types** check box.
   * - Column names
     - Bold
     - You can sort the backups by server by clicking the **Server** column
       label.
   * - Combo box names
     - Bold
     - Select a name from the **Send to** list, or type a new name.
   * - Command button names
     - Bold
     - Select **Microsoft Exchange** and then click **Next**.
   * - Command names, menu
     - Bold
     - To re-enable the system, select **Enable System** from the **System
       Actions** menu.
   * - Database names
     - Bold
     - Start by creating a new database called **mytestdb**.
   * - Dialog box names
     - Regular text
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.
   * - Directory names
     - *(Public)* Bold

       *(Private)* Monospace
     - *(Public)* Place all the contents of the uncompressed **wordpress**
       directory (excluding the directory itself) into the **/web/content/**
       directory, which is the root directory of the site.

       *(Private)* Place all the contents of the uncompressed ``wordpress``
       directory (excluding the directory itself) into the ``/web/content/``
       directory, which is the root directory of the site.
   * - Field names
     - Bold
     - In the **Database Name** field, enter a database name identifier.
   * - File names and extensions
     - *(Public)* Bold

       *(Private)* Monospace
     - *(Public)* To remove the **vs\_quantum-api.cfg** file from the
       **haproxy.d** directory and retain it, you can move it to another
       directory.

       *(Private)* To remove the ``vs_quantum-api.cfg`` file from the
       ``haproxy.d`` directory and retain it, you can move it to another
       directory.
   * - Folder names
     - Bold
     - Copy the **index.php** file from your computer to the **content**
       folder.
   * - Glossary terms
     - Italic, by applying the ``:term:`` directive in RST

       This directive also links the term to the definition in the glossary.
     - Rackspace provides an *IaaS* solution through a variety of complementary
       *services*.
   * - Group box names
     - Bold
     - In the **Edit Signature** area, enter the text that you want to appear
       in your signature.
   * - GUI labels
     - Bold

       In RST, apply the ``:guilabel:`` directive.

       **Exception:** Show window, dialog box, wizard, page, panel, and screen
       names in regular text unless they need to be distinguished from the
       surrounding text. In such cases, use bold.
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.

       On the Choose Service page, select **Microsoft Exchange or compatible
       service**, and then click **Next**.

       Read the preliminary steps in the Configure Your Server wizard, and then
       click **Next**.
   * - Icon names
     - Bold
     - To verify which OS version you are running, click the **Apple** icon in
       the top-left corner and then select **About This Mac**.
   * - List box names and selections
     - Bold
     - From the **Account Type** list, select **Exchange 2007**.

       To view these settings, select **Configure Backup** from the **Backup
       Actions** list.
   * - Menu names, commands, and sequences
     - Bold

       In RST, apply the ``:menuselection:`` directive to sequences.
     - Right-click the volume and select **Take Offline**.

       From the **Outlook** menu, select **Preferences**.

       Select **Start > Control Panel**, and then click the **Mail** icon.
   * - Option button names
     - Bold
     - Select **Microsoft Exchange** and then click **Next**.
   * - Page names
     - Regular text
     - On the Preferences page, you determine how frequently you receive email
       about all the activity on your account: daily, weekly, or both.

       On the Server Settings page, click **Check Name**, type your password,
       and then click **OK**.
   * - Panes, named and unnamed
     - Regular text
     - To verify that your SSL binding works, select your website in the
       Connections pane (if it is not already selected) and then click **Browse
       *ipAddress* (https)** in the Actions pane.

       In the navigation pane, select **Composing Email**.
   * - Paths
     - *(Public)* Bold

       *(Private)* Monospace
     - *(Public)* The path to Perl is **#!/usr/bin/perl -w**.

       *(Public)* In the URI path
       **https://incident.api.rackspacecloud.com/v1/...**, the API version is
       1.

       *(Private)* The path to Perl is ``#!/usr/bin/perl -w``.

       *(Private)* In the URI path
       ``https://incident.api.rackspacecloud.com/v1/...``, the API version is
       1.
   * - Radio button names
     - Bold
     - Select **Microsoft Exchange** and then click **Next**.
   * - Sequences
       (menu, field)
     - Bold

       Use **>** to separate.

       In RST, apply the ``:menuselection:`` directive.
     - Select **Start > Control Panel**, and then click the **Mail** icon.

       You can find more documentation about RackConnect in the **Community >
       Discussions > RackConnect** section of the MyRackspace Portal.
   * - Tab names
     - Bold
     - In the Microsoft Exchange dialog box, click the **Connection** tab and
       then select the **Connect to Microsoft Exchange using HTTP** check box.
   * - UI labels
     - Bold

       In RST, apply the ``:guilabel:`` directive.

       **Exception:** Show window, dialog box, wizard, page, panel, and screen
       names in regular text unless they need to be distinguished from the
       surrounding text. In such cases, use bold.
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.

       On the Choose Service page, select **Microsoft Exchange or compatible
       service**, and then click **Next**.

       Read the preliminary steps in the Configure Your Server wizard, and then
       click **Next**.
   * - User input
     - Bold
     - In the Server text box, type **outlook**.
   * - Window names
     - Regular text
     - In the Network Connections window, right-click the private adapter and
       select **Properties**.
   * - Wizard names and wizard page names
     - Regular text
     - On the Welcome page of the Active Directory Domain Services Installation
       Wizard, ensure that the **Use advanced mode installation** check box is
       cleared, and then click **Next**.

Time
~~~~

You can show time by using either the 12-hour or 24-hour clock. The
preferred format for international audiences, and the format used in
most computer systems, is the 24-hour clock. Use the 24-hour clock when
possible. If the technology or interface that you are documenting shows
or uses the 12-hour clock, then be consistent with the interface.

24-hour clock
-------------

When you use the 24-hour clock to show time, use the following
guidelines:

-  Separate the hours, minutes, and seconds by using a colon.
-  Show the hours, minutes, and second with two digits each, even if the
   leading digit is 0.
-  If you need to show a time zone, use Coordinated Universal Time
   (UTC), and indicate the time-zone offset from UTC.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - 08:29:37
   * - 18:30:59
   * - 18:00:00 to 20:30:00
   * - 10:30:00 (UTC -6) (refers to CT)
   * - 12:00:00 (noon)
   * - 00:00:00 (midnight)

12-hour clock
-------------

When you use the 12-hour clock to show time, use the following
guidelines:

-  Separate the hours and minutes by using a colon. If the minutes are
   00, you do not need to show them unless you are showing a span of
   time that includes a time with minutes.
-  Use lowercase letters for abbreviations of ante meridiem (a.m.) and
   post meridiem (p.m.). Separate these abbreviation from the time with
   a space. Use periods in the abbreviations.
-  When specifying time zones, show both the spelled-out name and the
   abbreviation. Show the name in lowercase letters; use uppercase
   letters and no periods for the abbreviation.
-  Avoid references to standard and daylight saving time because the
   appropriate designation changes frequently. However, if you need to
   include such a reference, insert *S* (for standard) or *D* (for
   daylight) as the second character in the abbreviation.
-  When referring to 12 a.m., use *12 midnight* or just *midnight*. When
   referring to 12 p.m., use *12 noon* or just *noon*.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - 10:29 a.m.
   * - 6 p.m.
   * - 6:00 p.m. to 8:30 p.m.
   * - 10:30 a.m. central time (CT)
   * - 1:30 p.m. central standard time (CST)
   * - midnight

Titles and headings
~~~~~~~~~~~~~~~~~~~

This topic provides guidelines for creating titles and headings in
documentation.

-  `Capitalization of titles and
   headings <#capitalization-of-titles-and-headings>`__
-  `Article titles and headings <#article-titles-and-headings>`__
-  `API content titles and
   headings <#api-content-titles-and-headings>`__
-  `Tables of contents <#tables-of-contents>`__
-  `Table, figure, and example
   titles <#table-figure-and-example-titles>`__
-  `Text following titles and
   headings <#text-following-titles-and-headings>`__

Capitalization of titles and headings
-------------------------------------

Use *sentence-style capitalization* for most titles and headings,
including article, chapter, table, figure, and example titles, as well
as section and procedure headings. One exception is book titles, which
use *title-style capitalization*.

For capitalization guidelines, see
`Capitalization <../a-l-style-guidelines.html#capitalization>`__.

Article titles and headings
---------------------------

This section provides guidelines for titles of articles and headings
within articles. For capitalization guidelines, see `Capitalization of
titles and headings <#capitalizatin-of-titles-and-headings>`__.

-  `Titles of articles <#titles-of-articles>`__
-  `Headings in articles <#headings-in-articles>`__

Titles of articles
^^^^^^^^^^^^^^^^^^

Observe the following guidelines when you are creating titles for
stand-alone articles on the Support site or in other collections of
documentation:

-  Create succinct, meaningful, descriptive titles that do not rely on
   body text or other titles for their meaning (that are, in other
   words, independent of context). Users should be able to tell from a
   title whether the information in the article is relevant to their
   needs. Avoid ambiguous one-word titles, such as "Overview."

-  Place the most important words first in a title.

-  Create unique titles for all of the articles within a documentation
   collection. To differentiate between titles that would otherwise be
   identical, add qualifiers either grammatically (for example, by
   adding a prepositional phrase) or by setting them off with a colon.

-  Do not number titles to indicate their placement in a series of
   articles. Indicate the order of articles *within* the content of the
   article, referring users to information that they should have read
   previously before reading the current article. Use links to provide
   navigation to preceding and following articles in the series.

-  Do not end a title with punctuation, except a question mark (when
   appropriate).

-  Avoid "telegraphic" language (in which omitted items, such as
   articles, can make text cryptic). Include articles, prepositions, and
   punctuation as needed for clarity. However, avoid using an article
   (*a*, *an*, or *the*) as the first word in a title.

-  Avoid showing both an abbreviation and its spelled-out term in a
   title. To help control the length of titles, show the abbreviation in
   the title and then define it in the first paragraph of the article.

-  If you show a literal term (such as a command or option name) in a
   title, follow it with an appropriate noun.

-  Do not include trademark symbols in titles. Show the symbol on the
   first use of the trademark in text.

-  Use a consistent grammatical structure for titles of specific types
   of articles:

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Article type
     - Grammatical structure
     - Examples
   * - Conceptual
     - Any grammatical structure that is appropriate, except a verb, gerund, or
       infinitive.
     - Linux distributions

       Best practices for backing up your data: Cloud Block Storage versus
       Cloud Backup
   * - Step-by-step instructions (a task)
     - An imperative verb.
     - Identify network interfaces on Linux

       Prepare data disks on Performance Cloud Servers running Windows

       Set up Mobile Sync For Webmail: iPhone and iPad
   * - Tutorial or high-level process
     - A gerund.
     - Understanding logrotate: Configuring and testing Customizing Apache web
       logs
   * - FAQ
     - A descriptive noun or noun phrase, followed by *FAQ*.
     - Rackspace Cloud Billing FAQ

       Scheduled images FAQ
   * - Reference
     - A plural noun or a noun phrase.
     - Permissions matrix for Cloud Networks

       Rackspace Auto Scale glossary
   * - Troubleshooting
     - A grammatical structure that is appropriate for the type of content. A
       troubleshooting topic can contain task, tutorial, concept, or reference
       information.
     - Troubleshooting alarms

       Service troubleshooting on Linux

Headings in articles
^^^^^^^^^^^^^^^^^^^^

Observe the following guidelines when you are creating headings within
articles:

-  Start with the highest level of heading that is approved for headings
   (for example, h3), and do not skip heading levels. Exceptions are
   made for questions within FAQ topics or terms within glossaries,
   which can use lower-level headings for formatting.

-  Avoid using more than two levels of heading within an article. If you
   use more than two levels of heading, consider whether the article is
   complex enough to be divided into two or more articles.

-  Do not use a heading as the first text in an article. Body text must
   intervene between the article title and the first heading.

-  Do not "stack" headings. Text should always intervene between
   headings. Ensure that such text is meaningful. If it is just filler
   text, consider whether you can restructure the article.

-  Avoid using only a single heading in an article. If you find that you
   have a single heading, consider whether you can reorganize the
   article to either eliminate the heading or add a second one.

-  Do not apply font treatments (bold, italics, or monospace) to text in
   a heading.

-  Do not include trademark symbols in headings. Show the symbol on the
   first use of the trademark in text.

-  Do not end a heading with a colon or period.

-  For guidelines about headings within task topics, see `Tasks and
   procedures <#tasks-and-procedures>`__.

API content titles and headings
-------------------------------

This section provides guidelines for creating titles and headings within
API content. For capitalization guidelines, see `Capitalization of
titles and headings <#capitalization-of-titles-and-headings>`__.

-  `Book titles <#book-titles>`__
-  `Section titles and headings <#section-titles-and-headings>`__

Book titles
^^^^^^^^^^^

Use title-style capitalization for titles that indicate a traditional
"book" title. For example, Developer Guide. For detailed capitalization
guidelines, see `Capitalization of titles and
headings <#capitalization-of-titles-and-headings>`__.

Section titles and headings
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Observe the following guidelines when you are creating section titles
and headings within sections.

-  Create succinct, meaningful, descriptive titles and headings, and
   place the most important words first.

   -  If possible, limit titles and headings to 60 characters for
      legibility in the TOC pane.

   -  Ensure that each title and heading are unique within a given content
      set.

   -  Consider that titles and headings are written within the context of
      the content set in which they are presented. Therefore, you can
      usually omit "context-setting" terms. For example, if the content set
      is about servers, you can usually omit "for servers" from the title
      or heading. (For example, "Attach a network to a server" can be
      shortened to "Attach a network" with no loss of clarity.)

-  Avoid "telegraphic" language (in which omitted items, such as
   articles, can make text cryptic). Include articles, prepositions, and
   punctuation as needed for clarity. However, avoid using an article
   (*a*, *an*, or *the*) as the first word.

-  Avoid showing both an abbreviation and its spelled-out term in a
   title or heading. To help control the length of titles and headings,
   show the abbreviation in the title or heading and then define it in
   the first paragraph of the section.

-  If you show a literal term (such as a command or option name) in a
   title or heading, follow it with an appropriate noun.

-  Do not end a title or heading with a colon or period. If the title or
   heading is in the form of a question, end it with a question mark.

-  Do not apply font treatments (bold, italics, or monospace) to text in
   a title or heading.

-  Do not include trademark symbols in titles or headings. Show the
   symbol on the first use of the trademark in text.

-  Avoid having only a single section title or heading. If you find that
   you have a single section or subsection, consider whether you can
   reorganize the information to either eliminate the title or heading,
   or add a second one.

-  Avoid having more than two levels of sections. If you use more than
   two levels of sections, consider whether you can reorganize to make
   the structure flatter.

-  Do not "stack" titles or headings. Text should always intervene
   between them. Ensure that such text is meaningful. If it is just
   filler text, consider whether you can restructure the content.

-  Use a consistent grammatical structure for titles of specific types
   of sections:

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Section type
     - Grammatical structure
     - Examples
   * - Conceptual
     - Any grammatical structure that is appropriate, except a verb, gerund, or
       infinitive.
     - Core concepts

       How Cloud Monitoring works

       Limitations of detaching from Rackspace networks
   * - Step-by-step instructions (a task)
     - An imperative verb.
     - Sign up for a Rackspace Cloud account

       Authenticate with the nova client
   * - Reference
     - A plural noun or a noun phrase.
     - Environment variables for the nova and supernova clients

       Restore operations

       cURL command summary
   * - High-level process or tutorial
     - A gerund.
     - Working with your first message queue
   * - Troubleshooting
     - A grammatical structure that is appropriate for the type of content. A
       troubleshooting topic can contain task, tutorial, concept, or reference
       information.
     - Troubleshooting

Tables of contents
------------------

In addition to using the preceding guidelines when creating titles and
headings, observe the following guidelines when creating a table of
contents (TOC) for a collection of content:

-  Entries in the TOC should link only to sections in the content. Do
   not include a link to an outside resource in the TOC.

-  The text of a TOC entry must match the text of the title or heading
   to which it links. If the link needs to be shorter, revise the the
   title or heading to be shorter.

-  Do not manually format the TOC. TOC formatting must be consistent and
   controlled by the code.

Table, figure, and example titles
---------------------------------

As a general rule, tables, figures, and examples should have titles
(also called captions). However, tables, figures, and examples in
procedures and tutorials do not normally require titles.

When creating titles for tables, figures, and examples, use the
following guidelines:

-  Use sentence-style capitalization. For detailed guidelines, see
   `Capitalization of titles and
   headings <#capitalization-of-titles-and-headings>`__.

-  Do not start a title with an article (*a*, *an*, or *the*).

-  Do not end a title with a period.

-  Place the title above the table, figure, or example, not below it.

-  Make titles concise and descriptive:

   -  Avoid using a title that duplicates an article or section title.
   -  Ensure that no two titles are identical. To distinguish between the
      titles that are similar, add a qualifier.

-  Do not include trademark symbols in titles.

Text following titles and headings
----------------------------------

Body text must follow titles and section headings. Do not follow a title
or heading directly with another heading.

The body text of a section or article must be independent from the title
or heading text. Don't use a title or heading as an antecedent in the
sentence that follows it. Put another way, be sure to repeat the subject
in the first sentence that follows the title or heading, rather than
using a pronoun that refers to the title or heading as its antecedent.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Do not use
   * - **Identify network interfaces on Linux**

       This article briefly describes how to identify which network interfaces
       on a Linux server are associated with which IP addresses.
     - **Identify network interfaces on Linux**

       This article briefly describes how to do this.

Trademarks
~~~~~~~~~~

Using Rackspace trademarks correctly protects Rackspace brands and
intellectual property, and promotes our reputation. Using third-party
trademarks correctly protects Rackspace from legal action.

Rackspace Legal has created comprehensive guidelines for using
trademarks at Rackspace. To get a comprehensive view of trademarks, read
the `21-page
PDF <https://one.rackspace.com/pages/worddav/preview.action?fileName=RACKSPACE-%2327629-v1-Rackspace_Trademark_Guidelines.pdf&pageId=72684499>`__.
If you are interested in only what you need to know to comply with
guidelines in your documentation, review the guidelines in this topic.

Examples of trademarks
----------------------

Following are examples of Rackspace trademarks:

-  Fanatical Support
-  Rackspace (when used in connection with service names)
-  Rackspace Managed Hosting
-  RackConnect

For a complete list, see the `Rackspace Trademark
List <https://www.rackspace.com/information/legal/tmlist>`__.

Following are examples of third-party trademarks that are often used in
our content: - Apache - Enterprise Linux - Linux - OpenStack - Python -
Red Hat - SQL Server - Ubuntu

If you need to verify whether a name is a trademark, see that company's
website.

Trademark usage guidelines
--------------------------

Use the following guidelines when showing Rackspace and third-party
trademarks in documentation.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Guideline
     - Example — Use
     - Example — Do not use
   * - Show a trademark exactly as it is shown by the owning company (Rackspace
       or third-party). Do not change the capitalization or abbreviate the
       trademark.

       Abbreviations are acceptable only if they are used by the owning company
       and also trademarked.
     - This article describes the process of backing up a Microsoft SQL Server
       2008 database. These actions need to be completed by the Administrator
       user or by a user who is part of the SQL Server Admin user group.
     - This article describes the process of backing up an MS SQL Server 2008
       database. These actions need to be completed by the Administrator user
       or by a user that is part of the MS SQL Admin user group.
   * - Use trademarks as adjectives on first use in the text of an article or
       chapter, and as often as possible after that.

       After first use, you can use the trademark as an noun if it is clear
       that you are referring to that trademark.

       Do not use a trademark as a verb.
     - Each cloud server has a single private IP address. When you use the
       RackConnect solution, if you need direct access to the cloud server from
       the Internet, you can use the public IP assigned to the server in
       RackConnect.
     - Each cloud server has a single private IP address. When you use the
       RackConnect, if you need direct access to the cloud server from the
       Internet, you can use the public IP assigned to the RackConnected cloud
       server.
   * - Do not combine a trademark with any other term, including another
       trademark. For example, do not attach a trademark to another term by
       using a hyphen or slash.
     - On Linux, Mac OS X, and other operating systems based on UNIX, you
       usually use the ssh command to connect to a server via SSH.
     - On Linux, Mac OS X, and other UNIX-based operating systems. you usually
       use the ssh command to connect to a server via SSH.
   * - Do not use a trademark as a possessive or as a plural. If necessary,
       form a possessive or plural from the noun that follows the trademark
       (which is used as an adjective).
     - The packaged version of NGINX from Ubuntu uses a sites-available and
       sites-enabled layout in the same manner as an Apache installation based
       on Debian.
     - Ubuntu's packaged version of NGINX uses a sites-available and
       sites-enabled layout in the same manner as a Debian-based Apache
       installation.
   * - Always distinguish a third-party trademark from a Rackspace product name
       or trademark. Generally you can do this through ensuring that words
       intervene between the trademarks.

       Show trademarks of different companies together only if a license or
       agreement exists between the two companies. In such cases, use italics
       to distinguish one trademark from the other. You can generally do this
       just on first use of the two terms together in the document or article.
     - The version of MySQL installed on Cloud Sites that use Windows
       technology is currently MySQL Connector version 5.2.5.

       The Rackspace Cloud Storage App for Microsoft SharePoint enables you to
       work with files inside of Rackspace Cloud Files alongside SharePoint
       content.
     - The version of MySQL installed on Windows Cloud Sites is currently MySQL
       Connector version 5.2.5.

       The Rackspace Cloud Storage App for Microsoft SharePoint enables you to
       work with files inside of Rackspace Cloud Files alongside SharePoint
       content.
   * - Always use *Fanatical Support* as a trademark. Do not use *fanatical*
       outside of the trademark. Also, always distinguish this trademark from
       surrounding text by using bold and italics (in RST, apply the
       ``:bolditalic:`` directive). Show a registered trademark symbol on first
       use.

       For more information, see the `Rackspace Trademark Guidelines PDF from
       Legal
       <https://one.rackspace.com/pages/worddav/preview.action?fileName=RACKSPACE-%2327629-v1-Rackspace_Trademark_Guidelines.pdf&pageId=72684499>`__.
     - We provide :bolditalic:`Fanatical Support` ®.
     - Our support is fanatical.

URLs and domain names
~~~~~~~~~~~~~~~~~~~~~

Some samples, such as those related to the Customer Service Layer API,
include a sample customer's URL or email address. Do not invent a fake
domain name for this purpose. Even if that name is not registered today,
someone might claim it tomorrow. Instead, use a domain name permanently
reserved for the purpose of demonstration and documentation.
**example.com** and **example.org** are reserved globally by the
Internet Assigned Numbers Authority (IANA).

Because the domain named **example.com** and the user named *Joe User*
do not and never will exist, it is safe to use the email address
**joe.user@example.com**.
