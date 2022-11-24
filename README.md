## Pull the Image ##

```docker pull erelozturk/nci-blockchain-ca```


## Run the image that you just pulled ##

```docker run --name ncilab02 -p 8090:8080 nci02```

## Run the curl commands ##

This transfers ETH:
```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9347d21dAFD97A175e16C74894101D59a0BD861c", "amount":"0.05"}' http://localhost:8090/eth```

This transfers token:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9347d21dAFD97A175e16C74894101D59a0BD861c"}' http://localhost:8090/token```

