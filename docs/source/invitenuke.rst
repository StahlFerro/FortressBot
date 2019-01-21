*****************
InviteNuke
*****************

iconfig
---------------
Checks the auto invite nuke settings of the server.


....

iexchannel
---------------
InviteNuke Exception Channels: View, add or remove text channels that will be excluded from the InviteNuke auto-deletion

.. code::

	]iexchannel [< add | remove | clear >] [text channels ...] (text channels parameter accepts channel tags or ids)

Examples:

- ``]iexchannel``
  displays all of the exception channels

- ``]iexchannel add #general #announcements``
  add channels by tags

- ``]iexchannel add 337732153281434124 2169764985762936789``
  add channels by ids

- ``]iexchannel remove #games #general``
  remove chanels

- ``]iexchannel clear``
  removes all of the channel exceptions

Both User and FortressBot must have Manage Messages permission for adding and removing exception channels


....

iexinvite
---------------
InviteNuke Exception Invites: View, add or remove invite links that will not be auto-deleted from the server

.. code::

	]iexinvite [< add | sync | remove | clear | expireclear >] [invites ...]

Examples:

- ``]iexinvite``
  displays all of the invites in the exception list

- ``]iexinvite add https://discord.gg/guide https://discord.gg/code``
  add invites

- ``]iexinvite sync``
  adds the invites of the current server into the exception list

- ``]iexinvite remove https://discord.gg/events https://discord.gg/discord-api``
  remove invites

- ``]iexinvite clear``
  removes all invites in the exception list

- ``]iexinvite expireclear``
  removes all invites that are expired in the exception list

Both User and FortressBot must have Manage Messages permission for adding and removing exception invites


....

iexrole
---------------
InviteNuke Exception Roles: View, add or remove roles that will bypass the InviteNuke auto-deletion

.. code::

	]iexrole [< add | remove | clear >] [roles ...] (roles parameter accepts role names or ids)

Examples:

- ``]iexrole``
  displays all of the exception roles

- ``]iexrole add @Moderator @Staff``
  add roles by tags

- ``]iexrole add 337732158137434124 413976498576293889``
  add roles by ids

- ``]iexrole remove @Developer @Proficient``
  remove roles

- ``]iexrole clear``
  removes all of the role exceptions

Both User and FortressBot must have Manage Messages permission for adding and removing exception roles


....

imode
---------------
Changes the InviteNuke's mode.

.. code::

	]imode < normal | mute | kick | ban >

- ``normal``
  : Delete invite links

- ``mute``
  : Delete invite links and mutes the user posting them (requires Manage Roles permission)

- ``kick``
  : Delete invite links and kicks the user posting them (requires Kick Members permission

- ``ban``
  : Delete invite links and bans the user posting them (requires Ban Members permission)

Both User and FortressBot must have Manage Messages permission for every modes, and additional permissions stated above for mute, kick and ban




....

ioff
---------------
Deactivates the automatic InviteNuke.

Both User and FortressBot must have Manage Messages permission


....

ion
---------------
Activates the automatic InviteNuke.

Both User and FortressBot must have Manage Messages permission


....

istring
---------------
Changes the InviteNuke's response string.

.. code::

	]istring [message]

Examples:

- ``]istring DONOTADVERTISEYOUCHEEKYSCRUB``
  (max characters: 700)

- ``]istring --reset``
  (reset to default)

Both User and FortressBot must have Manage Messages permission


