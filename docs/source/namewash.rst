*****************
NameWash
*****************

nwash
---------------
Assign a standard ASCII-fied and/or dehoisted nickname to a user, which is derived from it's original username

.. code::

	]nwash < dehoist | asciify | full > (users ...)

Examples:

- ``]nwash dehoist @User``
  

- ``]nwash full @User1 @User2 "User name3"``
  

Both User and FortressBot must have Manage Nicknames permission


....

nwasheveryone
---------------
Similar to nwash, but targets everyone in the server

.. code::

	]nwasheveryone < dehoist | asciify | full >

Example:

``]nwasheveryone dehoist`` 
Both User and FortressBot must have Administrator and Manage Nicknames permission


....

nwconfig
---------------
Display's this server's auto-NameWash configuration

The different Modes define the behavior of the NameWash

- ``Dehoist``
  : Remove hoisting characters on a user's name

- ``Asciify``
  : Converts non-standard ascii characters of a user's name into standard ascii characters

- ``Full``
  : Dehoists and Ascii-fies names simultaneously


....

nwhoistchars
---------------
Changes the NameWash's hoisting characters.

.. code::

	]nwhoistchars [character...]

Examples:

- ``]nwhoistchars !.[]{}%$``
  (max characters: 50)

- ``]nwhoistchars --reset``
  (reset to default)

Both User and FortressBot must have Manage Nicknames permission


....

nwmode
---------------
Changes the behavior of the auto-NameWash

.. code::

	]nwmode < dehoist | asciify | full >

Example:

``]nwmode asciify`` 
The different Modes define the behavior of the NameWash

- ``Dehoist``
  : Remove hoisting characters on a user's name

- ``Asciify``
  : Converts non-standard ascii characters of a user's name into standard ascii characters

- ``Full``
  : Dehoists and Ascii-fies names simultaneously


....

nwoff
---------------
Deactivates the automatic NameWasher.

Both User and FortressBot must have Manage Messages permission


....

nwon
---------------
Activates the automatic NameWasher.

Both User and FortressBot must have Manage Messages permission


....

swash
---------------
ASCII-fy and/or remove hoisting characters from a given string.

.. code::

	]swash < dehoist | asciify | full > (text)

Examples:

- ``]swash asciify "Я ø"``
  

- ``]swash full !ΣЯ``
  




