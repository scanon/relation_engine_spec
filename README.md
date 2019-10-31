# Relation Engine Spec

This repo holds the [stored queries](stored_queries), collection [schemas](schemas), and [subgraphs](subgraphs) for the relation engine graph database service.

These specifications are used by the [Relation Engine API](https://github.com/kbase/relation_engine_api)

* **Stored queries** are stored [AQL queries](https://docs.arangodb.com/3.3/AQL/index.html) that can be used
by KBase apps to fetch data from the database.
* **Schemas** are [JSON schemas](https://json-schema.org/) that define what form of data can be stored in
the database's collections.
* **Subgraphs** are groupings of vertex and edge collections into a semantically related sub-graph of data.

The additional configuration found in **/aliases.yaml** defines a set of custom names assigned to one or more collection names. This lets us abstract the database collection names, allowing us to rename underlying collections without breaking APIs.

## Development

### Running tests

Run tests with `make test`.
