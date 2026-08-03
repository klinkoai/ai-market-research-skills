# Klinko API Overview

All Klinko Skills will use one secure public API and the same Klinko intelligence layer. Skills differ in the question they ask, the workflow they follow, and the structure of the result they present.

## Public contract

The public API documentation will define:

- Authentication
- Query endpoint
- Request fields
- Response schema
- Error codes
- Rate limits
- Versioning and compatibility

## Status

The API base URL, endpoint path, request schema, response schema, error model, and rate limits are being finalized. They are intentionally not invented in this repository.

## Boundary

The public contract will document only what developers and Agents need to call Klinko safely. Private data infrastructure, internal datasets, processing systems, and server-side implementation remain outside the public interface.

