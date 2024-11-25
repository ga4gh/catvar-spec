.. _design-decisions:

Design Decisions
!!!!!!!!!!!!!!!!

Cat-VRS contributors confronted numerous trade-offs in developing this
specification. As these trade-offs may not be apparent to outside
readers, this section highlights the most significant ones and the
rationale for our design decisions, including the following.

*Check back on this page for more content as development progresses!*

Machine Readable Specifications
###############################

The machine readable Cat-VRS is written using `JSON Schema
<https://json-schema.org/>`_.

The schema itself is written in YAML (|vrs_yaml|) and converted to individual
JSON files for each class in the schema (|vrs_json|).

Contributions to the schema MUST be written in the YAML document.

General Principles
##################

* **Error handling is intentionally unspecified and delegated to
  implementation.**  Cat-VRS provides foundational data types that
  enable significant flexibility.  Except where required by this
  specification, implementations may choose whether and how to
  validate data.  For example, implementations MAY choose to validate
  that particular combinations of objects are compatible, but such
  validation is not required.

* **Cat-VRS uses** `snake_case
  <https://simple.wikipedia.org/wiki/Snake_case>`__ **to represent
  compound words.** Although the schema is currently JSON-based (which
  would typically use camelCase), Cat-VRS itself is intended to be neutral
  with respect to languages and database.

* **Optional attributes start with an underscore.** Optional
  attributes are not part of the value object.  Such attributes are
  not considered when evaluating equality or creating computed
  identifiers.