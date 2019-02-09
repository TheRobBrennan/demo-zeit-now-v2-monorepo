# Welcome
This project is intended to serve as a lightweight example for working with a monorepo that can be deployed to [Zeit Now 2.0](https://zeit.co/now).

You can view a [live demo](https://demo-monorepo-nowv2.now.sh) at [https://demo-monorepo-nowv2.now.sh](https://demo-monorepo-nowv2.now.sh)

This demo has been based off the original tutorial created by Zeit at [https://github.com/zeit/now-examples/tree/master/monorepo](https://github.com/zeit/now-examples/tree/master/monorepo)

**TL:DR** This is a monorepo consisting of a NextJS application which invokes four (4) separate back-end APIs - one written in Go, one written in NodeJS, one written in PHP, and one written in Python - that return the current time. In our `now.json` file, we have a routes key that will handle routing for our Monorepo. The contents from `www` will live at our root `/`, and the contents from `api` are mapped to `/api`

## Cheat sheet
```
// Step 1 - Create the project
$ mkdir api
  // Create api/go/index.go
  // Create api/node/index.js
  // Create api/php/index.php
  // Create api/python/index.py

$ mkdir www
  // Create package.json
  // Create pages/index.js
  // Create components/time.js
  // Create next.config.js

// Step 2 - Create `now.json` for deployment to Zeit Now v2

// Step 3 - Deploy to now
$ npm run deploy

```