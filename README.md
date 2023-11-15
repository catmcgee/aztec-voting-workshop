# Simplest Private smart contract | Developed for Nethermind Summit @ Devconnect 2023
Find gist for workshop [here](https://gist.github.com/catmcgee/98482a5cd9cf737fa109afdd436e4913).

# Prerequisites
* Aztec sandbox
`/bin/bash -c "$(curl -fsSL 'https://sandbox.aztec.network')"`
(for this you need Docker)
* Aztec-cli
`npm install -g @aztec/cli`

# Compile
In `contracts/voting`
```bash
aztec-cli compile .
```

# Deploy
After compilation, with sandbox running
```bash
aztec-cli deploy ./target/Voting.json --args <admin_address>
```
You can find existing acount addresses in the running sandbox output