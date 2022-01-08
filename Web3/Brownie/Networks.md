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

## Add new networks examples
```bash
brownie networks add Ethereum ganache-local host=http:/0.0.0.0:8545 chainid=1337
```

```bash
brownie networks add development mainnet-fork cmd=ganache-cli host=localhost fork=https://eth-mainnet.alchemyapi.io/v2/6lND9dYAUQ1RopEt1jKP-map_7NjuKMS accounts=10 mnemonic=brownie port=8545
```

## Delete Internal networks
```bash
brownie networks delete mainnet-fork
```