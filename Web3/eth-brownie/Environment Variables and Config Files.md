# .env and config.yaml example

## .env file 
```
export WEB3_INFURA_PROJECT_ID=YourProjectID
export PRIVATE_KEY=YourPrivateKey
```

## brownie-config.yaml
```yaml
dotenv: .env
wallets:
  from_key: ${PRIVATE_KEY}
```