# Decentralized Star Notary Service - Starter Code
* StarNotary: 0x84732c3102ca0215e2acaea1fd839a264c26281a
* ERC-721 Token Name: "starNotary Token"
* ERC-721 Token Symbol: "SNT"

# Instruction
This project is based on truffle v4.
## Download
```bash
$ git clone https://github.com/fido2478/dapp_notary.git
```

## Configuration
Make sure you have a right configuration on truffle.config by adding rineby network.
```javascript
rinkeby: {
  provider: function() {
    return new HDWalletProvider("<12 words mnemonic>", "4dfinfura address")
    
  },
      network_id: '4',
      gas: 4500000,
      gasPrice: 10000000000,
}
```

## Execution
On the backend side, open a terminal and run the following 
```bash
StarNotary$ truffle develop (to initialize a truffle project)
truffle(develop)> compile
truffle(develop)> test
truffle(develop)> migrate --reset --network rinkeby
```
On the frontend side, open another termninal and run the following
```bash
StarNotary$ truffle run dev
```