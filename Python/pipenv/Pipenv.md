# Pipenv
---
Automatically creates and manages a virtualenv for your projects, as well as adds/removes packages from your Pipfile as you install/uninstall packages. It also generates the ever-important Pipfile.lock, which is used to produce deterministic builds

## Pipenv installation Ubuntu
```bash
sudo apt install pipenv
```
<br><br>

## Pipenv usage 
### To create a virtual environment for the project
```bash
pipenv install
```

### To activate it
```bash
pipenv shell
```

### To install packages
```bash
pipenv install <package_name>
```

<br><br>
## Get the path where virtual environment is installed
```bash
pipenv --venv
```
