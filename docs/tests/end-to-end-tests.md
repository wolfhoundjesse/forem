---
title: End to End Tests
---

# End to End Tests

[Cypress](https://www.cypress.io/), a javascript based framework, is used for
end to end (E2E) testing. Tests and associated utilities are within the
`cypress` directory.

In addition to Cypress, we use
[cypress-testing-library](https://github.com/testing-library/cypress-testing-library).
This provides custom Cypress commands and utilities to improve how E2E tests are
written. dom-testing-library and preact-testing-library are already used for
[front-end tests](frontend-tests.md), which both offer a similar API in the
context of testing a Preact or Stimulus component. All these tools are part of
the [Testing Library](https://testing-library.com) family.

## Running Tests Locally

From the command line:

1. Ensure everything is up to date by running `bin/setup`
2. Run `yarn e2e` to start E2E testing. You will be prompted to set up the end
   to end (E2E) test database. Type `y` or `Y` to install the E2E test database.
   Typically this is a one time thing.

```bash
yarn run v1.22.5
$ bin/e2e
Do you need to set up your end to end (E2E) testing database? Answer yes if this is your first time running E2E tests on your local machine or you need to recreate your E2E test database. (y/n)
```

The E2E test database will install.

```bash
Setting up the E2E database before running E2E tests...


Dropped database 'PracticalDeveloper_test'
Created database 'PracticalDeveloper_test'

...
```

3. The Cypress test runner will open.
