# Setup config.yaml

##1- .env file 
Add private key and Infura:
```
export WEB3_INFURA_PROJECT_ID=YourProjectID
export PRIVATE_KEY=YourPrivateKey
```

##2- brownie-config.yaml
### Add .env
```yaml
dotenv: .env
```

### Add private key
```yaml
wallets:
  from_key: ${PRIVATE_KEY}
```

### Add dependencies example
```yaml 
dependencies:
  # - <organization/repo>@<version>
  - smartcontractkit/chainlink-brownie-contracts@1.1.1
compiler:
  solc:
    remappings:
      - '@chainlink=smartcontractkit/chainlink-brownie-contracts@1.1.1'
```