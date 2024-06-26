# JSON-Schema-Spec
Specification: https://json-schema.org/draft/2020-12/json-schema-core.html

Authors:

- Austin Wright
- Henry Andrews
- Ben Hutton
- Greg Dennis

Published: 16 June 2022

Metaschema: https://json-schema.org/draft/2020-12/schema

Implementations: https://bowtie.report/#/dialects/draft2020-12

Status: Stable

## Introduction

[Add texts here]

## Access all data connected to draft 2020-12

- Specifications
  - Core: [draft-bhutton-json-schema-01](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-01.html) ([changes](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-01.html#appendix-G))
  - Validation: [draft-bhutton-json-schema-validation-01](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-validation-01.html) ([changes](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-validation-01.html#appendix-C))
  - Relative JSON Pointer: [draft-bhutton-relative-json-pointer-00](https://tools.ietf.org/html/draft-bhutton-relative-json-pointer-00) ([changes](https://tools.ietf.org/html/draft-bhutton-relative-json-pointer-00#appendix-A))
  - Published: 16-June-2022
- General use meta-schemas
  - [JSON Schema meta-schema](https://json-schema.org/draft/2020-12/schema)
  - [JSON Hyper-Schema meta-schema](https://json-schema.org/draft/2020-12/hyper-schema) (2019-09 Hyper-Schema with 2020-12 Validation)
  - [JSON Hyper-Schema Link Description Object meta-schema](https://json-schema.org/draft/2020-12/links)
- Individual vocabulary meta-schemas
  - [Core Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/core)
  - [Applicator Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/applicator)
  - [Validation Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/validation)
  - [Unevaluated Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/unevaluated)
  - [Format Annotation Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/format-annotation)
  - [Format Assertion Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/format-assertion)
  - [Content Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/content)
  - [Meta-Data Vocabulary meta-schema](https://json-schema.org/draft/2020-12/meta/meta-data)
- Output schemas
  - [JSON Schema recommended output schema](https://json-schema.org/draft/2020-12/output/schema)
- Output examples
  - [JSON Schema verbose output example](https://json-schema.org/draft/2020-12/output/verbose-example)

### Obsolete Draft 2020-12 Documents

_These were updated without changing functionality or meta-schemas due to a few errors and unclear sections._

- Core: [draft-bhutton-json-schema-00](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-00.html) ([changes](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-00.html#rfc.appendix.G))
- Validation: [draft-bhutton-json-schema-validation-00](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-validation-00.html) ([changes](https://json-schema.org/draft/2020-12/draft-bhutton-json-schema-validation-00.html#rfc.appendix.C))

## Release Notes

### 2020-12 Release Notes

The previous draft (2019-09) introduced a lot of new concepts including `$recursiveRef`/`$recursiveAnchor`, `unevaluatedProperties`/`unevaluatedItems`, vocabularies, and more. Since then, these new features have seen multiple implementations and usage in real schemas. This draft is mostly dedicated to changes related to applying the lessons we've learned about implementing and using these new features in the wild.

This document attempts to put information most useful to schema authors toward the top and information for implementation authors toward the bottom.

### Changes to items and additionalItems

The keywords used for defining arrays and tuples have been redesigned to help lower the learning curve for JSON Schema. Since the `items` keyword was used for both types, we would often see people mistakenly defining a tuple when they meant to define an array and not understand why only the first item in the array was validating.

The `items` and `additionalItems` keywords have been replaced with `prefixItems` and `items` where `prefixItems` has the same functionality as the array-of-schemas for of the old `items` and the new `items` keyword has the same functionality as the old `additionalItems` keyword.

Although the meaning of `items` has changed, the syntax for defining arrays remains the same. Only the syntax for defining tuples has changed. The idea is that an array has items (`items`) and optionally has some positionally defined items that come before the normal items (`prefixItems`).

Here are some examples to illustrate the changes.

[Basically, copy and paste the release note into this section.]



# Navigation Menu Proposals.

## Idea 1.

##### Intro or Overview

##### Versions

- 2020-12
- 2019-09
- Draft 07
- Draft 06
- Draft 05

##### Specification Links

##### Migration

##### Release Notes

##### JSON Hyperschema

---

## Idea 2.

##### Overview

##### Versions

- 2020-12
- 2019-09
- Draft 07
- Draft 06
- Draft 05

##### Specification Links

##### Migration

##### Release Notes

- 2020-12
- 2019-09
- Draft 07
- Draft 06
- Draft 05

##### JSON Hyperschema

---

## Idea 3.

##### Overview

##### Specification Links

##### Versions

- 2020-12
- 2019-09
- Draft 07
- Draft 06
- Draft 05

##### Migration

##### Release Notes

##### JSON Hyperschema

# Overview section

This section contains all the details you need to effectively use the Specification documents.

### Specification Links

This document explains the complex numbering and naming system for drafts and meta-schemas.

### Versions

### Migration

Our migration guides on how to upgrade to newer JSON Schema draft versions.

### Release Notes

Our release notes gives you an overview of all the changes done in each draft.

### JSON Hyperschema

---

Understanding JSON Schema draft names and numbers

[Add text here]



