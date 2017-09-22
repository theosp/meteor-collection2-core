# aldeed:collection2-core

Part of aldeed:collection2. See https://github.com/aldeed/meteor-collection2

## Additions to aldeed:collection2 introduced in this fork:

Introduced a new method to Mongo Collections prototype 'allowSchemaCustomFields()'
that pass the allow_custom_fields option to collection's SimpleSchema (existing
one and those that will be created later).

The `allow_custom_fields` option of SimpleSchema introduced in a fork of
SimpleSchema available under: https://github.com/MeteorSpark/meteor-simple-schema

By passing this option to a created SimpleSchema, fields that aren't part of
the schema won't be filtered and won't be considered as invalid.
