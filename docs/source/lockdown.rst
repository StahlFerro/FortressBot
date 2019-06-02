*****************
Lockdown
*****************

!!serverlock
---------------
Locks all the text channels in a server, preventing anyone without Administrator permissions to chat.

.. code::

	]!!serverlock [reason]

Example:

``]!!serverlock mass raid`` 

Both User and FortressBot must have Administrator permission


....

!!serverunlock
---------------
Unlocks all the locked text channels in a serverUsage: ``]!!serverunlock``

Both User and FortressBot must have Administrator permission

⚠ WARNING: THIS COMMAND WILL UNLOCK READ-ONLY CHANNELS, IT'S RECOMMENDED TO CAREFULLY UNLOCK ALL TEXT-CHANNELS ONE BY ONE USING ``]!chatunlock``


....

!chatlock
---------------
Locks a channel, preventing anyone without an administrator role to post messages.

.. code::

	]!chatlock (channel) [reason]

Example:

``]!chatlock #general too much spamming`` (lockdown reasons are optional)

Both User and FortressBot must have Administrator permission


....

!chatunlock
---------------
Unlocks a locked channel.

.. code::

	]!chatunlock (channel)

Example:

``]!chatunlock #general`` 

Both User and FortressBot must have Administrator permission


....

!reactionlock
---------------
Disable reactions in a channel for everyone except Administrators

.. code::

	]!reactionlock (channel) [reason]

Example:

``]!reactionlock #general 3manyreactions5me`` (reactionlock reasons are optional)

Both User and FortressBot must have Administrator permission


....

!reactionunlock
---------------
Re-enable reactions in a channel

.. code::

	]!reactionunlock (channel)

Example:

``]!reactionunlock #general`` 

Both User and FortressBot must have Administrator permission


