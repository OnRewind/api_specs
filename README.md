# On Rewind Api Specifications
[![Build Status](https://travis-ci.org/onrewind/api_specs.svg?branch=master)](https://travis-ci.org/onrewind/api_specs)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)


On Rewind API specifications (in OpenAPI/Swagger) used in [doc-api.onrewind.tv](http://doc-api.onrewind.tv)
Every updates converts the open api specs into slate markdown and then publish the static website in gh-pages branch.

## Prerequisites

- docker
- node.js >= 8

## Installation

-  clone this project
- `npm install`
- `npm run docker:init`

## Usage

The following commands are available using `npm run`:

 - `openapi:compile` : compile split openapi spec files into one
 - `openapi:watch` : open a swagger ui preview in your browser, hot reload enabled if you modify any specs
 - `slate:init` : transpile openapi spec into slate spec and copy slate resources into tmp folder, should be run for any changes
 - `slate:preview`: open a slate preview in your browser, based on content in tmp folder
 - `slate:compile` : compile all files to build a slate static site into dist folder, based on content in tmp folder
 - `docker:init` : build docker image needed for slate
 - `dist` : combine commands to generate openapi spec and static site in one go

## License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

Thanks to the following projects/organization that helps us writing better documentation :)

* [swagger](https://swagger.io/)
* [widdershins](https://github.com/Mermade/widdershins)
* [docker](https://www.docker.com/)
* [slate](https://github.com/lord/slate)
* and other libraries defined in `package.json`
