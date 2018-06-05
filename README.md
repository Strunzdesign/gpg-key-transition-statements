# gpg-key-transition-statements
Transition statements for migrating to new GPG keys from existing ones

## What is this?
When migrating to new GPG keys, a chain of trust must be maintained from the old keys to the new ones.

The statements in this repository are signed with both the new and old keys and can be verified as being
authentic by downloading them (or cloning the repository) and running:

```gpg XXXXXXXX-transition-statement.txt.asc```
  
Both the old and new GPG keys will remain in public keyservers indefinitely, though old keys will
be revoked (and publicly displayed as such) shortly after their transitions are completed.

In some cases, the signature from the new keys may use a subkey of the new key, so the key ID shown
in the signature may not match the key ID of the parent key. *This is okay*; you can validate this
by looking up the parent key and finding the subkey contained in it.

## Key Migrations
Key migration statements this repository contains:

* 8900A8F5 (superseded 2018-06-04) => 8E6CD3D7
* 4074488B (superseded 2018-06-05) => 8E6CD3D7
