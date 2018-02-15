Sample Data
---

A simplified data model to get started.
This intermediary format consists of a 
set of nodes and a set of links.

All nodes have at least an `id` (string UUID), and 
`type` (string). Arbitrary properties can be
added to nodes in addition to these two properties.
A schema for each `type` defines which additional
properties are allowed.

Links must have a `source` (string UUID), `target`
(string UUID), and `type`. 
Arbitrary properties can be
added to links in addition to these three properties.
A schema for each `type` defines which additional
properties are allowed.

## Example

The example data provided in `example.json` was
parsed and extracted from the source file
in `source-data/rin-sample-01.xml`.

Example node:

```
{
    "type": "m-rin:Party",
    "id": "f890b9b4-1c6a-4235-b4dd-d51e0fc5d931",
    "ISNI": "0000 0001 0992 4566",
    "FullName": "Geoff Emerick",
    "FullNameIndexed": "Emerick, Geoff",
    "IsOrganization": "false"
}
```

Example link:

```
{
    "source": "99e8e6e5-da96-4804-b7ac-75e42219cbaa",
    "target": "d7112323-f426-483e-a7ec-1696195d2b71",
    "type": "ContributorReference",
    "role": "Musician",
    "instrument": "Voice"
}
```
