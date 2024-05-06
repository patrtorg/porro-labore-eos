# @nahkies/openapi-code-generator

![CI/CD](https://github.com/patrtorg/porro-labore-eos/actions/workflows/ci.yml/badge.svg)
[![npm](https://img.shields.io/npm/v/@nahkies/openapi-code-generator.svg)](https://www.npmjs.com/package/@nahkies/openapi-code-generator)

`@nahkies/openapi-code-generator` is a CLI tool that aims to generate high quality typescript client SDK's,
and API server scaffolding (routing, validation, serialization) from OpenAPI 3 specifications.

Currently, [OpenAPI 3.0](https://swagger.io/specification/v3), [OpenAPI 3.1](https://swagger.io/specification/),
and [TypeSpec](https://typespec.io/) are supported an input specifications.

<!-- toc -->

- [Documentation](#documentation)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

<!-- tocstop -->

## Documentation

Visit https://openapi-code-generator.nahkies.co.nz/ for detailed documentation including
quick start guides and reference material.

The documentation is built using NextJS / Nextra, and deployed using Github pages.
You can contribute to it in [./packages/documentation](./packages/documentation)

## Project Structure

The repository is structured as a mono repo of several npm packages that work together under [./packages](./packages):

- [openapi-code-generator](./packages/openapi-code-generator)
- [typescript-axios-runtime](./packages/typescript-axios-runtime)
- [typescript-fetch-runtime](./packages/typescript-fetch-runtime)
- [typescript-koa-runtime](./packages/typescript-koa-runtime)

The `openapi-code-generator` package is the main package, whilst the others are supporting packages used at runtime by
the code output by some of the templates.

Integration test definitions live in [./integration-tests-definitions](./integration-tests-definitions) and the generated
code output to [./integration-tests](./integration-tests)

Scripts to refresh the test data live in [./scripts](./scripts)

## Contributing

Contributing guidelines can be found in [./CONTRIBUTING.md](./CONTRIBUTING.md).

An overview of the codebase architecture is [available here](https://openapi-code-generator.nahkies.co.nz/reference/architecture)

## License

See [./LICENSE](./LICENSE)
