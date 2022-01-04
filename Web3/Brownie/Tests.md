# Tests
---

## Run tests
```bash
brownie test
```
Everything we can do with `brownie test` comes directly from `pytest`. Tools are the same!

### If we want to test a single function:
```bash
brownie test <func_name>
```
### Debug with python shell:
```bash
brownie test --pdb
```
### More verbose tests: 
```bash
brownie test -s
```