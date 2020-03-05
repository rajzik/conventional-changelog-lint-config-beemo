# @rajzik/conventional-changelog-lint-config-beemo

Config for [beemo preset](https://github.com/rajzik/conventional-changelog-beemo).

## Getting started

```sh
# Install commitlint cli and conventional config
npm install --save-dev @commitlint/cli @rajzik/conventional-changelog-lint-config-beemo
# For Windows:
npm install --save-dev @rajzik/conventional-changelog-lint-config-beemo @commitlint/cli

# Configure commitlint to use conventional config
echo "module.exports = {extends: ['@rajzik/conventional-changelog-lint-config-beemo']}" > commitlint.config.js
```

To lint commits before they are created you can use Husky's 'commit-msg' hook:

```json
{
  "husky": {
    "hooks": {
      "commit-msg": "commitlint -E HUSKY_GIT_PARAMS"
    }
  }
}
```

## Further instructions

[commitlint](https://github.com/conventional-changelog/commitlint)
