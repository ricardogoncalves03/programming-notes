# Networks
---
Whenever we deploy to a network, the default is **Ganache-CLI: development**.
Development networks are temporary. The contracts and transactions sent 
on these blockchains are deleted after our script completes.

**Ethereum networks** are gonna be the persistent ones

## Get a list of networks
```bash
brownie networks list
```

## Connect to Infura 
In your .env file, type in:
```
export WEB3_INFURA_PROJECT_ID=YourProjectID
```

## Activate .env (Need to test which one worked)
### 1.
Add this in your _brownie-config.yaml_
```yaml
dotenv: .env
```
### 2. If it gives an error such as:
`ValueError: Unable to expand environment variable in host setting:`

Try:

```bash
source .env
```
### 3 - If it still doesn't work, try to add in your deploy script
```python
from dotenv import load_dotenv

load_dotenv()
```

## Deploy to Rinkeby
```bash
brownie run scripts/deploy.py --network rinkeby
```