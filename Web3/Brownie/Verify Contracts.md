# Verify contracts - Etherscan
---

# Etherscan - create account

https://etherscan.io/login

## API-KEYs

In *My Profile*, go to *API-KEYs* and click *Add* 

## Add Api-Key Token in .env
```
export ETHERSCAN_TOKEN=W853U1U8HE9WQ682QXVEDTS31KZY9PBVR8
```

## In your deploy script, add publish_true=True 
Example:
```python
fund_me = FundMe.deploy({"from":account}, publish_source=True)
```
## Etherscan contract should look like this when deployed
![Etherscan contract deployed correctly](/images/contract_deployed.png)