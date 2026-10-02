# Security and document data handling

This repository contains prompt instructions, office document processing code, and publishing/install helper scripts. Their presence does not establish that outputs are correct or that data stays local.

## Before use

- Read each skill, referenced source, and executable script before enabling or running it.
- Treat contracts, resumes, invoices, spreadsheets, and business documents as sensitive.
- Use synthetic documents during initial testing.
- Inspect MCP tools, dependencies, network requests, file access, and temporary-file behavior before supplying private data.
- Verify generated calculations, legal language, citations, and document rendering independently.
- Do not commit API keys, client files, extracted text, or generated sensitive documents.

The Office MCP package declares document processing libraries and a `test` script, but no test result or data-retention guarantee is asserted here. See the package's own documentation before deployment.

## Reporting

Do not publish secrets, personal information, or exploit details in public issues. Use GitHub private vulnerability reporting if enabled, or contact the repository maintainer privately. Include the affected path, impact, and safe reproduction steps.

The repository's root MIT license may not cover separately maintained materials or third-party references. Verify terms for each component before redistribution.
