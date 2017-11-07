# salt-hash-research

## Problems that salt/hash help to resolve:

- Plain Text can be hacked easily by dictionary attacks. 

- Stored plain text can be easily stolen using brute force.

- Just encryption is two way, with the encryption key a password can be easily decrypted.

- Hashing provides more protection; however, "Rainbow Table Attacks" can still access passwords.


## Overview

Salt:

Salt is randomly generated values that are added before hashing the value to help make the value more unique.
Salts are stored at the site (database/server) and can be "unique" to help prevent the values from being determined.

Hash:

Approach to storing passwords. One way function that represents the password the user has entered.
Hashing will always produce the same output.

Examples:

For example, if a user enters the word "apple":
Without salting, the password hash might be "B11NS".
The hash for any password of "apple" will always be represented as "B11NS".

Adding salt might make the hash look like "!B511N3!S".
If the salt is "unique" the values added to the hash are the salt.

