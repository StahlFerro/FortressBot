*****************
Utility
*****************

about
---------------
checks the stats of FortressBot


....

avatar
---------------
Displays a user's avatar.

.. code::

	]avatar [user]

Examples:

- ``]avatar``
  Displays your own avatar

- ``]avatar Lario``
  Displays Lario's avatar


....

changelog
---------------
Displays the details of the bot's latest update


....

embed
---------------
Creates an embedded message. Refer to the format below

.. code::

	]embed [title] [description] [thumbnailurl] [imageurl] (field1) (text1) (field2) (text2) ...\nTitle, description, thumbnailurl and imageurl can be blanked out by typing "".

Each field must have a corresponding text.


....

hasrole
---------------
Displays a list of all users that has a certain role.

.. code::

	]hasrole (role)

Example:

``]hasrole Staff`` 

....

invite
---------------
Generates an link to invite FortressBot


....

magnify
---------------
Enlarge an emote.

.. code::

	]magnify (emote)

Example:

``]magnify :thinking:`` 

....

ping
---------------
Checks the latency of the bot


....

roleinfo
---------------
Retreives info of a role, including it's permissions

.. code::

	]roleinfo (role)

Example:

``]roleinfo Moderator`` 

....

rolelist
---------------
Displays a list of every role in the server and how many users have them.

.. code::

	]rolelist [number]

Example:

``]rolelist 1`` 

....

roletable
---------------
Displays a table of server roles and their permissions.

.. code::

	]roletable < 1 - n >

Example:

``]roletable 1`` (page number)

....

serveremotes
---------------
Brings up a list of custom emotes a server have.


....

serverinfo
---------------
See server information


....

timestring
---------------
Display the timestring format that FortressBot uses when defining time


....

userinfo
---------------
Retrieves info of a user.

.. code::

	]uinfo [user]

Examples:

- ``]uinfo``
  Gets your own user information

- ``]uinfo Mario``
  Gets user information from user named Mario


....

userpermissions
---------------
Lists all of the permissions a user has in the current text channel.

.. code::

	]uperms [user]

Examples:

- ``]uperms``
  Gets your own list of channel permissions

- ``]uperms Jake``
  Gets Jake's list of channel permissions


