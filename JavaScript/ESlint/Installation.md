# ESlint

## Install ESlint
```bash
npm install eslint --save-dev

./node_modules/.bin/eslint --init
```

### .eslintrc.json file:
```json
{
    "env": {
        "commonjs": true,
        "es2021": true,
        "node": true
    },
    "extends": [
        "airbnb-base"
    ],
    "parserOptions": {
        "ecmaVersion": 13
    },
    "rules": {
        "no-console": "off"
    }
}
```
## If ESlint doesn't work and gives an error like:
```bash
Failed to load config "airbnb-base" to extend from.
```
**Install:**
```bash
npm install -g install-peerdeps
install-peerdeps --dev eslint-config-airbnb
install-peerdeps --dev eslint-config-airbnb-base
```
Source: https://stackoverflow.com/questions/69733256/failed-to-load-config-airbnb-to-extend-from-gitlab-ci