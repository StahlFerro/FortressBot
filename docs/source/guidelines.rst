***************
Guidelines
***************


Primer
----------------
As a moderation-oriented bot, it should be given the appropriate permissions on a server in order for it to operate its functions that require additional 
permissions. Upon joining a server, FortressBot would automatically have a role with the same name created in the server. Deleting this role while 
FortressBot is in the server is highly discouraged, as it would make it unable to function properly in the server.

A good understanding of discord's permission system and role hierarchy is recommended when setting up or using FortressBot's commands that requires 
managerial permissions, e.g., mute, kick, ban, message pruning or invitenuke commands; adjusting them to your server's set of roles and permissions.


Command Syntax
----------------

FortressBot's command syntax format is defined in this following example:

.. code::

    ]acommand (user) (users ...) [channel] [role] (timestring) < -fun | -serious | -relaxed > { 1 - 1337 }


- ``()`` Parentheses means the argument is required.
- ``[]`` Square brackets means the argument is optional. May contain other brackets inside it, marking them optional as well.
- ``<>`` Arguments enclosed between these are required options.
- ``{}`` Braces means a required number within the specified range. On the example above, it means it can be any number between 1 and 1337.
- ``user`` A discord user. Can be supplied with their tag, username, username#discrim, or user id. Nicknames are not allowed. Examples:

    - ``@StahlFerro``
    - ``StahlFerro``
    - ``StahlFerro#0055``
    - ``300611567874080769``

- ``channel`` A discord channel. Can be supplied by its tag or id. Examples:

    - ``#cool-channel``
    - ``455310436091428874``

- ``role`` A discord role. Must be supplied with its name or id. Examples:

    - ``Moderator``
    - ``487094250836852751``

- ``...`` One or more of the previous identifiers. Examples:

    - ``(users ...) -> ``@StahlFerro @Martin``
    - ``(channels ...)`` ->``#general #mod-logs #memes-room``
    - ``"Dellia Agate" @Marzinyu`` If you want to specify a user by their name and it has spaces, enclose them in double quotation marks
    - ``306467828729380874 332603467577425929``

- ``timestring`` See below section.

Syntax-less commands found in the documentation does not require arguments at all.


Timestrings
----------------

Timestring is a format that expresses time durations, and is FortressBot's default time format for commands.


Below is the format of a timestring

.. code::

    000.000y-111.111mo-222.22w-333.33d-444.44h-555.5m-666s

``y`` years, ``mo`` months, ``w`` weeks, ``d`` days, ``h`` hours, ``m`` minutes, ``s`` seconds

All of the 7 units of time above accepts numbers up to hundreds, but some has different decimal precision.
Years and months accepts up to 3 decimal numbers.
Weeks, days and hours accepts up to 2 decimal numbers.
Minutes only accepts up to 1 decimal number.
Seconds does not accept decimals at all

Examples:

- ``2h5m`` (2 hours and 5 minutes)
- ``4.5h`` or ``4h30m`` (4 hours and 30 minutes)
- ``1w1d`` or ``8d`` (8 days)
