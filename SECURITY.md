# Security policy

## Reporting a vulnerability

Please report security problems privately: on this repository's Security tab,
open Advisories and choose Report a vulnerability. Please don't open a public
issue for them.

## How the toolkit handles risk

- Credentials come from environment variables (see `.env.example`), never from
  files in this repository.
- The tools that can change a device or a NetBox record are dry runs until you
  pass `--apply`.
- Captured device configs belong in a separate private repository, never in this one.
