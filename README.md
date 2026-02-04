# cytoscape-extension-esm-analysis
Analysis on ESM support for Cytoscape.js extensions
# Cytoscape.js Extension ESM Analysis

This repository contains notes and observations from exploring how Cytoscape.js extensions are currently built and how they differ from the core Cytoscape.js build setup.

## Current Cytoscape.js Core Setup
- It uses Rollup as the build tool.
- It publishes ESM, CommonJS, and UMD builds.
- Uses modern 'exports' definitions in package.json.

## Current Extension Build Patterns
- Here most extensions use Webpack.
- Output is typically UMD/CommonJS only.
- Here ESM builds and 'exports' are usually missing

## Problems for ESM Users
- Extra bundler setup needed.
- ESM is hard to use in browser.
- Not easy for new contributors.

## What an ESM-First Extension Template Should Provide
- Rollup based build setup.
- ESM and CommonJS output.
- Standard package.json fields.
- Simple structure for beginners.

## Reference
- These observations are based on reviewing the Cytoscape.js core repository and a few commonly used extensions on GitHub.

