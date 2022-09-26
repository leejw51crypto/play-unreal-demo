# basic play2earn  example
`caution!!`  
`this is a work in progress. never meant for the production. please use for testing purpose`


## setup variable
- MYCRONOSRPC : https://evm-dev-t3.cronos.org
- MYCRONOSCHAINID : 338
- MYMNEMONICS : your mnemonics
    
## minting
- go to ./mint folder
- make install
- make 
- write down, MYCONTRACT721, MYCONTRACT1155 
  

## play2earn setup
- open ./Config/test.json
- example
```json
{
	"Erc721Contract": "0x7828B6E1b347101f3Dd21f72151C10e6962528Ab",
	"Erc721NftItems": [
		"78",
		"83",
		"88",
		"90"
	],
	"Erc721Holders":
	{
		"0x1b3727f7bdef3afe2f06a415a0b4925361915788": [
			"23",
			"29",
			"26"
		]
	},
	"Erc1155Contract": "0x7aD36bE5E24C7b8133D4a5689442f1C8c78A9998",
	"Erc1155NftItems": [
		"0",
		"1",
		"2"
	],
	"Erc1155Holders":
	{
		"0x1b3727f7bdef3afe2f06a415a0b4925361915788":
		{
			"0": ""
		}
	}
}
```
- modify Erc721Contract,  Erc1155Contract
- Erc721NftItems to reward
- Erc721Holders, Erc1155Holders information will be updated

## setup unreal project
- open CryptoFire.uproject to open unreal
- open Content/My/MyGameInstance
- setup CronosRpc, CronosChainId 
- example
```unreal
CronosRpc = "http://mynode:8545"
CronosChainId = "777"
```

## for test mnemonics
- can enter in `Start` scene
- or MyGameInstance MyMnemonics (for testing only)
- WalletSenderIndex for sender index
- WalletReceiverIndex for receiver index
  


  
