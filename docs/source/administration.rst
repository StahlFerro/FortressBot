*****************
Administration
*****************

!addrole
---------------
Adds a role to one or more users.

.. code::

	]!adr (role) (users ...)

Example:

``]!adr Moderator @User1 @User2 @User3`` 

(max: 50 users)

Both User and FortressBot must have Manage Roles permission


....

!ban
---------------
Bans a user.

.. code::

	]!ban (user) [reason]

Examples:

- ``]!ban @Eris``
  

- ``]!ban @Cyanlake For trolling others``
  (ban reasons are optional)

- ``]!ban 405001870160035842``
  (ban users that are not in the server by their ids)

Both User and FortressBot must have Ban Members permission


....

!clear
---------------
Removes a number of FortressBot's messages.

.. code::

	]!clear { 1- 100 }

Example:

``]!clear 70`` (default amount: 10)

Both User and FortressBot must have Manage Messages permission


....

!cmute
---------------
Create the ``Fortress Muted`` role for the ``]!mute`` command.

This role also generates a new permission on every channel. If you happen to create new text channels after you execute this command, and the Fortress Muted role channel permission is not in those channels, you can rerun this command to generate the missing permissions

Running this command also resets the Fortress Muted channel permissions to its default deny overwrites

Both User and FortressBot must have Manage Roles permission


....

!exportchat
---------------
Exports a number of messages of the channel into a json file sent via Direct Message

.. code::

	]!exportchat < 1 - 1000000 > [#channel]

Examples:

- ``]!exportchat 9001``
  Exports the last 9001 messages of the current channel and send them to the command issuer's DM

- ``]!exportchat 600 #mychannel``
  Exports the last 600 messages from channel #mychannel and send them to the command issuer's DM

Both User and FortressBot must have Administrator permission, and the User must enable DMs from server members


....

!kick
---------------
Kicks a user from the server.

.. code::

	]!kick (user) [reason]

Examples:

- ``]!kick @StahlFerro``
  

- ``]!kick @Delagate Spamming non stop``
  

Both User and FortressBot must have Kick Members permission


....

!massban
---------------
Bans multiple users at once.

.. code::

	]!massban (reason) (users ...)

Example:

``]!massban "Raiding and spamming" @User1  @User2  @User3`` 

(max: 50 users, use "" for no ban reason)

Both User and FortressBot must have Ban Members permission


....

!masskick
---------------
Kicks multiple users at once.

.. code::

	]!masskick (reason) (users ...)

Example:

``]!masskick "Raiding" @User1  @User2  @User3`` 

(max: 50 users, use "" for no kick reason)

Both User and FortressBot must have Kick Members permission


....

!mute
---------------
Mutes one or more users. Specify a timestring before the users for a temporary mute

.. code::

	]!mute [timestring] (users ...)

Examples:

 ``]!mute @User``

- ``]!mute @User1 @User2 @User3 ...``
  

- ``]!mute "Swag lord" "Blobman" "Luke Landrunner"``
  

- ``]!mute UserID1 UserID2 ...``
  

- ``]!mute 1.5h @User``
  

- ``]!mute 20m UserID1 UserID2 ...``
  

(max: 50 users)

You can look at the timestring format that FortressBot accepts by typing ``]timestring``

Both User and FortressBot must have Manage Roles permission


....

!mutelist
---------------
Displays detailed information of all muted users in the server

.. code::

	]!mutelist [csv]

- ``]!mutelist``
  Displays a pager of the mute list

- ``]!mutelist csv``
  Generates a csv file containing the mute list information

Both User and FortressBot must have Manage Roles permission


....

!nick
---------------
Sets a nickname for a user. Leaving the parameter blank resets their nickname.

.. code::

	]!nick (user) (newnickname)

Example:

``]!nick @user supernick`` 

Both User and FortressBot must have Manage Nicknames permission


....

!pin
---------------
Pins a message in a channel.

Examples:

- ``]!pin``
  Pins the latest message in a channel

- ``]!pin ASDFJKL``
  Pins the message ASDFJKL

Both User and FortressBot must have Manage Messages permission


....

!prune
---------------
Deletes messages in a channel with the given amount.

.. code::

	]!prune { 1 - 1000000 } [< user_id | "string" | -links | -images | -bots | -reactions >]

Examples:

- ``]!prune 40``
  Deletes 40 messages

- ``]!prune 20 cheesecake``
  Deletes 20 messages containing the string 'cheesecake'

- ``]!prune 13 @Shusui``
  Deletes 13 of Shusui's messages

- ``]!prune 37 223161712092774402``
  Deletes 37 of messages made by a user with that id.

- ``]!prune 90 -links``
  Deletes 90 messages containing clickable links

- ``]!prune 60 -images``
  Deletes 60 images/attachments

- ``]!prune 80 -bots``
  Deletes 80 messages sent by bots

- ``]!prune 35 -reactions``
  Deletes reactions in the last 35 messages (max last 100 messages)

Both User and FortressBot must have Manage Messages permission

Both User and FortressBot must also have Administrator permission to delete more than 1000 messages at once


....

!removerole
---------------
Remove a role from one or more users.

.. code::

	]!rmr (role) (users ...)

Example:

``]!rmr Officer @User1 @User2 @User3`` 

(max: 50 users)

Both User and FortressBot must have Manage Roles permission


....

!rolepurge
---------------
Removes all of a user's roles. This doesn't remove the ``Fortress Muted`` role.

.. code::

	]!rolepurge (user)

Example:

``]!rolepurge @User`` 

Both User and FortressBot must have Manage Roles permission


....

!unban
---------------
Unbans a user.

.. code::

	]!unban (userid)

Example:

``]!unban 223161712092774402`` 

Both User and FortressBot must have Ban Members permission


....

!unmute
---------------
Unmutes one or more users

.. code::

	]!unmute (users ...)

Examples:

 ``]!unmute @User``

- ``]!unmute @User1 @User2 @User3``
  

- ``]!unmute "MLG Man" "Obi Twelve" "Merya"``
  

- ``]!unmute userid1 userid2``
  

(max: 50 users)

Both User and FortressBot must have Manage Roles permission


....

!unpin
---------------
Unpins the latest pinned message.

Both User and FortressBot must have Manage Messages permission


