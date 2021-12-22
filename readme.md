# Mint NFT by using Candy machine

### Check candy machine cli 
```ts-node ./metaplex/js/packages/cli/src/candy-machine-cli.ts help upload```

### Step1 upload
```ts-node ./metaplex/js/packages/cli/src/candy-machine-cli.ts upload ./metaplex/solchick-assets --env devnet --keypair ./keys/alice.json```

output \
candy machine with publickey: 89CBeAbyoiFg9gDRcptsKE16MYmnfHnuuFGCpJFS2PTx

### Step2 check
```ts-node ./metaplex/js/packages/cli/src/candy-machine-cli.ts verify --keypair ./keys/alice.json --env devnet```

### Step3 Create
```ts-node ./metaplex/js/packages/cli/src/candy-machine-cli.ts create_candy_machine --env devnet --keypair ./keys/alice.json -p 1```

### Step4: Mint
```ts-node ./metaplex/js/packages/cli/src/candy-machine-cli.ts mint_multiple_tokens -k --env devnet --keypair ./keys/alice.json --number 3```

#### mint_one_token 
```ts-node ./metaplex/js/packages/cli/src/candy-machine-cli.ts mint_one_token -k ./keys/alice.json --env devnet```

https://solscan.io/token/FGTSxd5R5VgN7gPNCjkXRVSHKAwNjgZhTEfjiVbBtQ4k?cluster=devnet

#### Mint NFT on Mainnet 
Use <--env mainnet-beta> instead of <--env devnet>
