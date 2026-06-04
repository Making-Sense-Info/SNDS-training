# VTL Training

This repository contains training materials for [VTL 2.1](https://sdmx-twg.github.io/vtl/v2.1/).

## Notes

VTL does not define how to load/persist data.

In the VTL scripts provided in this repository, we use the following notations to represent data import and export:

- import: `foo.bar`, in an expression, means you read the `bar` data source located in `foo`(path/method defined elsewhere, according to the tool)
- export: `baz.quux` in a persistent assignment, means you will persist the `quux` dataset in `baz` (path/method defined elsewhere, according to the tool)

Example:

```vtl
baz.quux <- foo.bar [keep aa][rename aa to bb];
```

## SNDS

- [SNDS trainings](./snds/README.md)