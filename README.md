# pouchdb-internals

- `sync`
  - instantiates `Sync`
    - creates `push` and `pull` replication processes using `replicate`
  - https://github.com/pouchdb/pouchdb/blob/master/src/sync.js

## `AbstractPouchDB`

- https://github.com/pouchdb/pouchdb/blob/master/src/adapter.js
- `AbstractPouchDB.prototype.info` is a [template method][] which defers request for into to `_info` method

[template method]: https://en.wikipedia.org/wiki/Template_method_pattern

## Utilities  

- `adapterFun`
  - create a function which will be executed in context of a PouchDB object
  - https://github.com/pouchdb/pouchdb/blob/master/src/deps/adapterFun.js

- `getArguments`
  - https://github.com/calvinmetcalf/argsarray  
