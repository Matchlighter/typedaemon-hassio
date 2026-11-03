## 0.6.0

- 912c034 bump version
- 8de9fe3 Merge branch 'config-reload-watch' into 'master'
- 24e69ce Merge branch 'resumable-transformer-fixes' into 'master'
- eecebb4 config: survive atomic saves in file watcher; add dashboard Reload Config
- d1b0e65 resumable: address code review
- 4378991 resumable: bounded suspend wait, partial save, named failure reasons (td-639)
- f5a5b7e hoist: per-iteration envs for loop bindings captured by closures (td-8tr)
- c2b9507 visit: leave nested async fns inside resumable bodies as plain async (td-epy)
- c85f5fe resumable: preserve aliasing/cycles across the persisted executor frame (td-5et)
- 83b3cf2 emit: support ??, spread, templates, optional chains containing await (td-j9y, td-y9x, td-x5k, td-m63)
- 72d8c0e emit: support for-of / for-await-of containing await (td-20n)
- 90ff4ce emit: support optional and destructured catch bindings (td-0gb, td-pmb)
- 23193be hoist: rewrite only references to the resumable fn's own bindings (td-lu4)
- 2f761bf visit: support destructured/default/rest method params (td-6is)
- 1342bcb hoist: don't rewrite non-reference identifiers (keys, labels, shorthand) (td-1im)
- 6bd8062 hoist: support destructured var declarations (td-ak1)
- 114cdd6 test: resumable transformer emit/hoist coverage
