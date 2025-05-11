# openssl-rand

> Generate pseudo-random bytes.
> More information: <https://docs.openssl.org/master/man1/openssl-rand>.

- Generate 16 random bytes and output them in hexadecimal (e.g., for a 128-bit key):

`openssl rand -hex 16`

- Generate 32 random bytes and output them in Base64 (e.g., for a 256-bit key):

`openssl rand -base64 32`

- Generate a custom number of random bytes and write them to a file (binary output):

`openssl rand -out {{path/to/file}} {{num_bytes}}`

- Generate a specific number of random bytes (e.g., {{num_bytes}}) suitable for a cryptographic key, using specific providers, and output in hexadecimal:

`openssl rand -hex -provider default -provider fips {{num_bytes}}`

- Seed the random number generator from a specific file before generating {{num_bytes}} random bytes in hexadecimal:

`openssl rand -rand {{path/to/seed_file}} -hex {{num_bytes}}`
