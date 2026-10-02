# Contributing to DivineAPI repositories

Thank you for helping improve the DivineAPI repositories. This guide applies to every public repository in the DivineAPI GitHub account.

## What we accept

| Contribution | How |
|---|---|
| README and documentation fixes (typos, broken links, unclear steps, wrong parameter names) | Open a pull request |
| New examples (another language, framework or use case for an existing endpoint) | Open a pull request that adds files under `examples/` |
| SDK code changes (`divineapi-python`, `divineapi-node`, `divineapi-php`) | Open an issue or a pull request; SDK code changes are reviewed by the DivineAPI engineering team before they are merged |
| Bug reports in the SDKs or examples | Open an issue with the bug report template |
| Feature ideas for the SDKs or examples | Open an issue with the feature request template |

## Where to ask instead

- **Questions about the API** (endpoints, parameters, responses, plans, billing, your account): use [support.divineapi.com](https://support.divineapi.com). Issues in these repositories are for the code and docs in the repository.
- **API reference**: [developers.divineapi.com](https://developers.divineapi.com)
- **Service status**: [status.divineapi.com](https://status.divineapi.com)
- **Security problems**: never in a public issue. See [SECURITY.md](SECURITY.md).

## Rules for pull requests

1. **No credentials.** Never commit an API key, auth token or `.env` file. Examples must read credentials from the `DIVINEAPI_API_KEY` and `DIVINEAPI_AUTH_TOKEN` environment variables, and show `YOUR_API_KEY` / `YOUR_AUTH_TOKEN` in docs.
2. **Facts only.** Use real endpoint paths, parameter names and response fields from [developers.divineapi.com](https://developers.divineapi.com). Do not add claims about accuracy, rankings or features that the docs do not describe.
3. **Run what you add.** Every new or changed example must run against the live API and succeed before you open the pull request. Paste the (trimmed) output in the pull request description, with credentials removed.
4. **Real responses.** If you add a response sample, use a real response, trimmed with `...`, keeping real field names and values.
5. **Match the request format.** Every call is a `POST` with `multipart/form-data`, the auth token in an `Authorization: Bearer` header and the API key in the `api_key` form field. On the hosts that always answer HTTP 200, check `success` in the body (`1` = OK).
6. **Keep changes small.** One topic per pull request makes review faster.
7. **Brand name.** The name is written "DivineAPI" (one word).

## Licence

Each repository states its licence in its `LICENSE` file (the SDKs, MCP repos and example repos use the MIT licence). By opening a pull request you agree that your contribution is released under the licence of the repository you contribute to. The DivineAPI name and logo are not covered by that licence.

## Code of conduct

Everyone taking part is expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md).
