*****************
Technical
*****************

base64
---------------
Encodes or decodes a string into/from base64.

.. code::

	]base64 < -e | -d > (text)

Examples:

- ``]base64 -e ayylmao``
  -e for encoding the text into base64

- ``]base64 -d bG1hb2F5eQ==``
  -d for decoding the base64 string into plain text


....

caesar
---------------
Encrypts or decrypts a text using the Caesar cipher.

.. code::

	]caesar < -e | -d > { -26 - 26 } (text)

Examples:

- ``]caesar -e 12 I am trained in ban warfare``
  Encrypt the text, shifting it 12 characters forward

- ``]caesar -d 9 jwm R'v cqn cxy vxmnajcxa rw cqn nwcran mrblxam javnm oxalnb``
  Decrypt the text, shifting it 9 characters backward


....

calc
---------------
Performs mathematical calculations

Examples:

- ``]calc (4+20) * (13/37)``
  Supported operators: + - * / ^

- ``]calc Sqrt(6)``
  

- ``]calc Pow(9,2)``
  

- ``]calc Round(PI) * Floor(4.16^2)``
  

More info on math expressions here:

<https://msdn.microsoft.com/en-us/library/system.math(v=vs.110).aspx>

See Methods and Fields section of the webpage


....

charinfo
---------------
Displays information of characters.

.. code::

	]charinfo (string)

Examples:

- ``]charinfo ∞``
  

- ``]charinfo #$%^&*``
  

Supports conversion of up to 30 characters at once


....

color
---------------
Previews a sample of a color.

Example:

``]color #0070FF`` (hash sign is optional)


....

ipcalc
---------------
IP calculator for class C subnets.

.. code::

	]ipcalc { 24 - 30 }

Example:

``]ipcalc 28`` (use CIDR number, range: 24-30)


....

nco
---------------
Converts any number from one numeral system to the others. The format of the number must correspond to the chosen option

.. code::

	]nco < -d | -h | -b | -o > (number)

Options: ``-d``: decimal, ``-h``: hexadecimal, ``-b``: binary, ``-o``: octal

Examples:

- ``]nco -d 1234678``
  

- ``]nco -h 7f8bdf5``
  


....

strcomp
---------------
Lists the amount of characters in a string

.. code::

	]strcomp (string)

Example:

``]strcomp STAhL F3Rr0`` 


....

strgen
---------------
Generates a random string of the given length (min 1, max 1000) with options

.. code::

	]strgen { 1 - 1000 } [< -n | -u | -l >]

Examples:

- ``]strgen 12``
  generates a random 12-character string of uppercase, lowercase and numbers

- ``]strgen 7 -n``
  generates a random 7-character string of numbers only

- ``]strgen 20 -u``
  generates a random 20-character string of uppercase letters only

- ``]strgen 3 -l``
  generates a random 3-character string of lowercase letters only

Options can be mixed. For example: -ln generates both lowercase letters and numbers, -un generates both uppercase letters and numbers

PS: NEVER USE THIS AS A PASSWORD GENERATOR!


....

strlen
---------------
Returns the length of a string

.. code::

	]strlen (string)

Example:

``]strlen ABCDEFGHIJKL`` (returns 12)


....

time
---------------
Expresses the time in utc, and in another time zone additionally.

.. code::

	]time [{ -12 - 12 }]

Examples:

- ``]time``
  Current time in UTC

- ``]time -8``
  Current time in UTC and in GMT-8


