```sh
aws ec2 describe-spot-price-history --start-time=$(date +%s) --product-descriptions="Linux/UNIX" --query 'SpotPriceHistory[*].{az:AvailabilityZone, price:SpotPrice}' --instance-types c4.large
```
