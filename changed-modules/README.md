# changed-modules

_The `changed-modules` action, leverages `hpcc-systems/skip-duplicate-actions` action to calculate which component parts of the HPCC Platform repository have changed_

## Outputs

* workflows
* platform
* dockerfiles
* ecllibrary
* eclwatch
* docs
* testing
* initfiles
* other

**Note:**  To simplify the usage of the outputs, all values are either `true` or `''` (empty string), this allows the following github expression to work as expected:

```js
  if: ${{ xxx.yyy.outputs.eclwatch }}
```

