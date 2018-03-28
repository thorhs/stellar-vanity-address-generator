# Stellar Vanity
A simple CLI tool to generate Stellar vanity addresses.

**Vanity Address:** similar to a vanity license plate, a vanity cryptocurrency address is an
address where either the beginning (prefix) or end (postfix) is a special or meaningful phrase.
Generating such an address requires work. Below is the expected time and difficulty of finding
different length words in a vanity address (based on a more optimized algorthim/codebase).

![https://imgur.com/diotZ02.png](https://imgur.com/diotZ02.png)

## How to use:
```
use vanity_key::generate_vanity_key;

generate_vanity_key("A"); // Where A is the desired postfix.
```

This will continuously loop until a key with the desired postfix is found. Once the vanity address is found,
a tuble (public_key, private_key) will be returned. Note, this is a synchronous function.
