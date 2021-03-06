# salt-hash-research

code example: https://github.com/PrimeAcademy/psp_bcrypt/blob/master/app.js

## Problems that salt/hash help to resolve:

- Plain Text can be hacked easily by dictionary attacks. 

- Stored plain text can be easily stolen using brute force.

- Just encryption is two way, with the encryption key a password can be easily decrypted.

- Hashing provides more protection; however, "Rainbow Table Attacks" can still access passwords.


## Overview/Definitions

Salt:

Salt is randomly generated values that are added before hashing the value to help make the value more unique.
Salts are stored at the site (database/server) and can be "unique" to help prevent the values from being determined.

Hash:

Approach to storing passwords. One way function that represents the password the user has entered.
Hashing will always produce the same output.

Rainbow Table Attack:

this attack involves a pre-generated list of hash outputs/inputs that are able to be compared to hashed passwords to determine the values.

Examples:

For example, if a user enters the word "apple":
Without salting, the password hash might be "B11NS".
The hash for any password of "apple" will always be represented as "B11NS".

Adding salt might make the hash look like "!B511N3!S".
If the salt is "unique" the values added to the hash are the salt.


## Requirements

bcrypt package installed with node
