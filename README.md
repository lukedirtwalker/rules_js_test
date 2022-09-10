# Trying to run @redocly/cli with rules_js

```
bazel run -- @nodejs_host//:npx_bin pnpm@latest exec redocly --version
```

^ works correctly.

```
bazel run //:redocly
```

Fails with:
```
node:internal/modules/cjs/loader:936
  throw err;
  ^

Error: Cannot find module 'lodash.isequal'
```
