# ESlint

## Install ESlint
```bash
npm install eslint --save-dev

./node_modules/.bin/eslint --init
```

### .eslintrc.json file react example:
```json
{
    "env": {
        "browser": true,
        "es2021": true,
        "node": true
    },
    "extends": [
        "eslint:recommended",
        "plugin:react/recommended",
        "plugin:react/jsx-runtime"
    ],
    "parserOptions": {
        "ecmaFeatures": {
            "jsx": true
        },
        "ecmaVersion": "latest",
        "sourceType": "module"
    },
    "plugins": [
        "react"
    ],
    "rules": {
        "eqeqeq": "error",
        "no-trailing-spaces": "error",
        "object-curly-spacing": [
        "error", "always"
        ],
        "arrow-spacing": [
        "error", { "before": true, "after": true }
        ],
        "no-console": 0
    }
}
```
