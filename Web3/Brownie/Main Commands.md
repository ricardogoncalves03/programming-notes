# Main Commands
---

## Create new project
```bash
brownie init
```
If you installed Brownie with pipenv, run this command instead:
```bash
brownie init --force
```

## Compile code
```bash
brownie compile
```

## Deploy to a network (Ganache-CLI)
```bash
brownie run scripts/deploy.py
```
Whenever we deploy to a network, the default is Ganache-CLI: development
