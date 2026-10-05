# docugoat-data

Ciphertext-only store for [docugoat](https://github.com/brandy-savage/docugoat). Every file here is AES-256-GCM output produced in a browser; keys never touch GitHub.

- `envelopes/<id>/envelope.json` — sealed document (per-recipient key wraps + ciphertext)
- `envelopes/<id>/signatures/*.json` — encrypted signature bundles
- `envelopes/<id>/events/*.json` — encrypted audit events
- `vault/<id>.json` — an owner vault, encrypted under their username + passphrase

