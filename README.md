# nunu.ai API Reference Documentation

This repository contains the API reference documentation for nunu.ai, covering programmatic access to AI-powered game testing capabilities.

## Documentation Structure

The documentation is organized into the following sections:

### Overview
- **Introduction** - API overview, base URL, and response formats
- **Authentication** - API key management and security

### Runs API
Endpoints for managing test runs:
- `GET /runs` - List runs with filtering and pagination
- `POST /runs` - Start a test or test plan
- `GET /runs/{runId}` - Get detailed run information with artifacts
- `GET /runs/{runId}/bugs` - List bugs found in a run
- `POST /runs/stop` - Stop one or more running tests

### Builds API
Endpoints for managing game builds:
- `POST /builds/upload` - Initiate a multipart build upload
- `GET /builds/upload/parts` - Get presigned URLs for upload parts
- `POST /builds/upload/complete` - Complete the upload
- `DELETE /builds/upload` - Cancel an in-progress upload

## Local Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview documentation changes locally:

```bash
npm i -g mint
```

Run the development server from this directory:

```bash
mint dev
```

View your local preview at `http://localhost:3000`.

## Publishing Changes

Changes pushed to the default branch are automatically deployed to production via our GitHub app integration.

## Documentation Links

- **API Reference**: The documentation deployed from this repository
- **Main Documentation**: https://docs.nunu.ai (Nexus documentation)
- **Dashboard**: https://nunu.ai/nexus

## Troubleshooting

- If the dev environment isn't running: Run `mint update` to ensure you have the latest CLI version
- If a page loads as a 404: Ensure you're running in a folder with a valid `docs.json`

## Resources

- [Mintlify documentation](https://mintlify.com/docs)
- [nunu.ai website](https://nunu.ai)
- [GitHub](https://github.com/nunu-ai)
- [Discord community](https://discord.gg/nunu)
