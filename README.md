# React Api Client

A npm package for calling APIs in React.

## For building the package

```bash
npm pkg set main="lib/index.js" types="lib/index.d.ts" scripts.build="tsc" scripts.prepare="npm run build"
```

## Publishing

To publish a new version of the package:

1. Update the version in package.json

```bash
npm version patch
```

2. Publish to npm

```bash
npm publish
```

## For using the package

```bash
npm install react-api-client
```

## Usage

```ts
import { callApi } from "react-api-client";

const data = await callApi("https://jsonplaceholder.typicode.com/todos/1");
```

## License

React Api Client is licensed under the Apache License, Version 2.0. See the [LICENSE](./LICENSE) file for more details.