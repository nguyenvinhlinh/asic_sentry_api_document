# ASIC Sentry API Document

### Install

1. Install [Node JS](https://nodejs.org/).
2. Clone this repo and run `npm install` in the repo root.

### Usage

#### `npm start` or `npm exec redocly preview-docs -- --port 8086`
Starts the reference docs preview server.

#### `npm run build` or `npm exec redocly bundle -- openapi/openapi.yaml  -o dist/bundle.yaml`
Bundles the definition to the dist folder.

#### `npm run build-html` or `npm exec redocly build-docs --  --output dist/asic_sentry.html`
Build html file to serve with nginx.

#### `npm test`
Validates the definition.

## Build with docker and get files for nginx.
```
$ DOCKER_BUILDKIT=1 docker build -f  Dockerfile --target=release --output nginx-dist .
```
