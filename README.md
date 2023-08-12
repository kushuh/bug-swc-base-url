# Issue

Read the issue description here: https://github.com/swc-project/swc/issues/7800

## How to reproduce

Set `"@swc.core": 1.3.76` in package.json.

```bash
mnpm i
npm run registry:compile

# thread '<unnamed>' panicked at 'base_dir(.) must be absolute.
# Please ensure that `jsc.baseUrl` is specified correctly.'
```

Set `"@swc.core": 1.3.75` in package.json.

```bash
mnpm i
npm run registry:compile

# ... Compilation success
```
