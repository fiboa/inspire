# INSPIRE Extension Specification

- **Title:** INSPIRE
- **Identifier:** <https://fiboa.github.io/inspire-extension/v0.2.0/schema.yaml>
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
| inspire:id    | string | **REQUIRED**. INSPIRE-compliant ID, an absolute and fully resolvable URI. Example: `https://geodaten.nrw.de/id/inspire-lc-dgl/landcoverunit/6467974` |

## Contributing

See the [contributing guideline](CONTRIBUTING.md) for more details.
