# prisma-kysely

## 1.4.1

### Patch Changes

- 36393b6: Bugfix: revert to own generated type, that supports ColumnType

## 1.4.0

### Minor Changes

- 3288b72: Support @map statement for enum values (Thank you @jvandenaardweg 🔥🇳🇱)
- 299de40: Adds support for Kysely's `GeneratedAlways` through a new config parameter `readOnlyIds`. The generated type file no longer includes and exports the `Generated` generic.
- 66019e8: Brings back support for implicit many to many models after DMMF changes introduced in new version of Prisma

### Patch Changes

- 2659cc3: Now using narrower types for enum objects bringing `prisma-kysely`'s enums in line with `prisma-client-js` (Thank you @jvandenaardweg 🎉)

## 1.3.0

### Minor Changes

- a96f2d7: Add option to output runtime enums to a separate file (Thank you @juliusmarminge! 🇸🇪🎉)

## 1.2.1

### Patch Changes

- ff5bc59: Add object declarations for enums, that can be used (among other things) for runtime validation. Thanks @jvandenaardweg for the idea! 😎👍

## 1.2.0

### Minor Changes

- 533e41e: Pass Prisma comments on Prisma fields to the generated TypeScript types
- 8892135: Add support for field level @map and update core dependencies

## 1.1.0

### Minor Changes

- 7ab12d5: The first minor version bump 😮. Turns out some of the type maps were wrong. This update corrects `BigInt` and `Decimal` types for all dialects, and corrects the `DateTime` type for SQLite.

## 1.0.11

### Patch Changes

- 1cb96de: Update README

## 1.0.10

### Patch Changes

- Add support for CockroachDB (thanks to @yevhenii-horbenko 🥳)

## 1.0.9

### Patch Changes

- 3bb5d89: Add support for Kysely's camel case plugin

## 1.0.8

### Patch Changes

- e7ecabe: Adds Typescript as a primary dependency in order to fix issue #8

## 1.0.7

### Patch Changes

- 0a50f6f: Add support for @@map("...") statements (mapping models to different table names) and table names with spaces
