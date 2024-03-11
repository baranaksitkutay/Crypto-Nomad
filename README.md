# Crypto-Nomad
We are working to connect our home page with mint contract, work in progress.


![alt text]([http://url/to/img.png](https://cdn.discordapp.com/attachments/1144380746933477490/1216799180282925126/logo.png?ex=6601b38b&is=65ef3e8b&hm=3a6fe5eaa9e536bb139918327b3a248ee505fca7b02ef73c8a79db319cacfbd0&))

Sunum:
https://docs.google.com/presentation/d/1k-vxA8Zhqg_s5lz8ReCJkZkjRcYbXswqbXh0qsPgT3Q/edit?usp=sharing

For Main Page:
- yarn create next-app -e https://github.com/emreaksitkutay/Crypto-Nomad
- yarn dev

For Mint Contract:
Install Solana Tool Suite
https://docs.solana.com/cli/install-solana-cli-tools#windows
cmd /c "curl https://release.solana.com/v1.15.2/solana-install-init-x86_64-pc-windows-msvc.exe --output C:\solana-install-tmp\solana-install-init.exe --create-dirs"
solana --version
solana-keygen --version

Get current directory:
cd SimpleSolanaNFT

solana-keygen new --outfile C:\Users\User\Desktop\Metaplex\Owner.json

solana-keygen new --outfile C:\Users\User\Desktop\Metaplex\Creator.json
Do the below if you haven't setup config before
solana config set --keypair C:\Users\User\Desktop\Metaplex\Owner.json
solana config set --url https://api.devnet.solana.com
solana config get

solana airdrop 1 "" --url https://api.devnet.solana.com
solana airdrop 1 "" --url https://api.devnet.solana.com

Create Candy Machine Config File
./sugar create-config

Upload assets
./sugar upload

Deploy Candy Machine
./sugar deploy

[1/3] Creating collection NFT for candy machine

Collection mint ID: CD2dtKYKLhrPWz47iWKdpkdehKnapF1NQugD8Ks1qeTt

[2/3] Creating candy machine

Candy machine ID: Dh7dw1DFsQ7VpuyA8Eu3vS89kZ1d9LEebQj9QX6J4wfM

Verify Candy Machine Deployment and Setup
./sugar verify

Add Candy Guards
./sugar guard add
./sugar guard show

Setup KeyStrokes Candy Machine UI
cd '.\CandyMachineSite'
cp ..env.example .env

Update .env file with Candy Machine
npm install npm run dev
