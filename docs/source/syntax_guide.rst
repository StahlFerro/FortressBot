***************
Syntax Guide
***************

FortressBot's command syntax format are defined in this following example:

.. code::

    ]acommand (user) (users ...) [channel] [role] < -fun | -serious | -relaxed > { 1 - 1337 }


- ``()`` Parentheses means the argument is required.
- ``[]`` Square brackets means the argument is optional. May contain other brackets inside it, marking them optional as well.
- ``<>`` Arguments enclosed between these are required options.
- ``{}`` Braces means a required number within the specified range. On the example above, it means it can be any number between 1 and 1337.
- ``user`` A discord user. Can be supplied with their tag, username, username#discrim, or user id. Nicknames are not allowed. Examples:

    - ``@StahlFerro``
    - ``StahlFerro``
    - ``StahlFerro#0055``
    - ``300611567874080769``

- ``users ...`` One or more discord users. Similar with above rule. Examples:

    - ``@StahlFerro @Martin``
    - ``Argus Levia``
    - ``"Dellia Agate" @Marzinyu`` If you want to specify a user by their name and it has spaces, enclose them in double quotation marks
    - ``306467828729380874 332603467577425929``

- ``channel`` A discord channel. Can be supplied by its tag or id. Examples:

    - ``#cool-channel``
    - ``455310436091428874``

- ``role`` A discord role. Must be supplied with its name or id. Examples:

    - ``Moderator``
    - ``487094250836852751``

Syntax-less commands found in the documentation does not require arguments at all.
