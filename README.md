# README

This is a sphinx, sphinx-needs based T-req like requirement management system.

- subsystems as submodules (independent life cycle)
- protocols as submodules (independent life cycle)

It focusses on Medical Products that are composed of Hardware and Software.
The focus is on Software towards meeting the regulatory needs of ISO 62304.

It clearly distinguishes between:

- **Requirements** that are wishes the system shall fulfill, where ISO 62304
  requests it's verification.
- **Constraints** that are a-priory taken design decisions that cannot be undone.
- **Specifications** that are design decisions taken in the course of development.

## Guidance

- git is used to organize
  - revisioning/baselining, diffing
  - reviewing and approval by PR/by signoff
- sphinx with needs plugin is is used
  - to structure the documentation, provide browseable access
  - prevent broken links
  - compute traceability
  - prevent missing traces



### ID System

Identifier:

Form <TYPE>_<OPTIONAL CATEGORY>_<uniuqe number>

The type corresponds to the need item type, is much shorter as defined in
`conf.py` variable `needs_types`.

The identifier are documented in *Identifier Prefix glossary*.


### Directory Structure and toc tree

- each directory has a index page containing toctree only
  (toc tree without caption and 2 levels visibility)
- index in top level directories start with part headlines (*)
- detailed level headlines are (=)

## Building

### Prerequisites

1. Install python
2. Install sphinx and extensions, specifically sphinx-needs
```
python -m pip install -r requirements.txt
```

### Building

Build html in _build/html folder
```
python -m sphinx -M html docs _build
```

Run live
```
python -m http.server 8000 --directory ./_build/html

```


