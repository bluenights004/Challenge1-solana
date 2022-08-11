# Challenge 1 Solana - Airdrop test

Creating airdrop transaction to user's choice of wallet address

Detail instruction on how to do:

Keypairs and Airdrops
Challenge - Airdrop SOL
Now that you know how to submit a challenge, let's get started.

Modify the logic of the existing piece of code to get airdropped into an account of the user’s choice. To run the script, you can take the account address as a CLI parameter.

In the code snippet, you can see that the publicKey is being used to airdrop:

const fromAirDropSignature = await connection.requestAirdrop(
                new PublicKey(myWallet.publicKey),
                2 * LAMPORTS_PER_SOL
            );

This “myWallet.publicKey” should be replaced with the Public key entered by the user.


Another note, in order to properly execute the code, make sure the input data is a verified account public address in solana dev net.
Sample public address generated: Dd2SxYbVpnBHePctAv54PbQpuioznCUTGmSTq82G1GFL

Solana dev net link:
https://explorer.solana.com/address/Dd2SxYbVpnBHePctAv54PbQpuioznCUTGmSTq82G1GFL?cluster=devnet