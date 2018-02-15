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

