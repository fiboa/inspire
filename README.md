# INSPIRE Extension Specification

- **Title:** INSPIRE
- **Identifier:** <https://fiboa.github.io/inspire-extension/v0.1.0/schema.yaml>
- **Property Name Prefix:** inspire
- **Extension Maturity Classification:** Proposal
- **Owner**: @m-mohr

This document explains the INSPIRE Extension to the
[Field Boundaries for Agriculture (fiboa) Specification](https://github.com/fiboa/specification).

It adds support for a property that reflects the INSPIRE ID.

- Examples:
  - [GeoJSON](examples/geojson/)
  - [GeoParquet](examples/geoparquet/)
- [Schema](schema/schema.yaml)
- [Changelog](./CHANGELOG.md)

## Properties

The fields in the table below can be used in these parts of fiboa documents:

- [ ] Collection
- [x] Feature Properties

| Property Name | Type   | Description |
| ------------- | ------ | ----------- |
| inspire:id    | string | **REQUIRED**. INSPIRE-compliant ID, a absolute and fully resolvable URI. Example: `https://geodaten.nrw.de/id/inspire-lc-dgl/landcoverunit/6467974` |

## Contributing

All contributions are subject to the
[fiboa Code of Conduct](https://github.com/fiboa/specification/blob/main/CODE_OF_CONDUCT.md).
For contributions, please follow the
[fiboa contributing guideline](https://github.com/fiboa/specification/blob/main/CONTRIBUTING.md).

### Running tests

You'll need to install [nodejs and npm](https://nodejs.org/en/download/) to run the tests.
Alternatively, you can also use [yarn](https://yarnpkg.com/) instead of npm.
In this case replace all occurrences of `npm` with `yarn` below.
Additionally, you need Python >= 3.9 installed.

Afterwards, navigate to the root of the specification repository.
Now, install the required test software: `npm install` and `npm run init`

Finally, you can run all tests or subset of them:

- To run all tests: `npm test`
- To check the markdown run: `npm run check-docs`
- To check the examples run: `npm run check-examples`
