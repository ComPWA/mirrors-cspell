# cspell mirror

Mirror of
[cspell](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
package for [pre-commit](https://pre-commit.com), created with
[`pre-commit-mirror-maker`](https://github.com/pre-commit/pre-commit-mirror-maker).
See
[github.com/pre-commit/mirrors-prettier](https://github.com/pre-commit/mirrors-prettier)
for an example of a pre-commit hook for a Node.js package.

### Using cspell with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/ComPWA/mirrors-cspell
  rev: "" # Use the sha / tag you want to point at
  hooks:
    - id: cspell
```

By default, all files are passed to `cspell`. If you want to limit the file
list, adjust `types` / `files`:

```yaml
- id: cspell
  types:
    - javascript
    - python
```
