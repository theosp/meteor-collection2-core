## Change Log

### 1.2.1

Introduced a new method to Mongo Collections prototype 'allowSchemaCustomFields()'
that pass the allow_custom_fields option to collection's SimpleSchema (existing
one and those that will be created later).

The `allow_custom_fields` option of SimpleSchema introduced in a fork of
SimpleSchema available under: https://github.com/MeteorSpark/meteor-simple-schema

By passing this option to a created SimpleSchema, fields that aren't part of
the schema won't be filtered and won't be considered as invalid.

### 1.2.0

Support for SimpleSchema 2.0

### 1.1.1

- Fix merging of identical selector schemas (thanks @spencern)
- Fix attaching w/ "replace" option when switching between a selector and non-selector schema (thanks @paulbalomiri)
- Fix choosing of correct selector schema for cleaning inserts or updates that originate on the client (thanks @paulbalomiri)

### 1.1.0

Support for multiple schemas on the same collection. See aldeed:collection2 readme.

### 1.0.0

Initial release. Previously included in aldeed:collection2 package.
