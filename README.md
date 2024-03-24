# Overmind NFT Collection Smart Contract
This smart contract is designed to manage a collection of non-fungible tokens (NFTs) on the SUI blockchain, specifically tailored for the Overmind NFT Collection.

### Features
* Minting NFTs: Users can mint new NFTs by paying a specified amount of SUI coins. Each NFT has a unique name, description, and image.
* Combining NFTs: Users can combine two existing NFTs into a new one, with a new name, description, and image.
* Withdrawing Sales: The contract owner can withdraw the sales balance accumulated from NFT purchases.
* Burning NFTs: Owners of NFTs can burn (delete) their tokens.
### Smart Contract Functions
`init`
* Initializes the smart contract, transferring ownership of the MinterCap object to the sender.

`mint_nft`
* Mints a new NFT and transfers it to the recipient.
* Returns: Change coin.
1) recipient: Address of the recipient.
2) nft_name: Name of the NFT.
3) nft_description: Description of the NFT.
4) nft_image: Image of the NFT.
5) payment_coin: Coin used to pay for the NFT.
6) minter_cap: MinterCap object.

`combine_nfts`
* Combines two NFTs into a new NFT.
* Returns: New NFT object.
1) nft1: First NFT object.
2) nft2: Second NFT object.
3) new_image_url: Image of the new NFT.

`withdraw_sales`
* Withdraws the sales balance from the MinterCap object.
* Returns: Withdrawn coin.
1) minter_cap: MinterCap object.

`burn_nft`
* Deletes an NFT object.
1) nft: NFT object to burn.

### Getter Functions
`name`: Gets the name of an NFT.

`description`: Gets the description of an NFT.

`url`: Gets the image URL of an NFT.
## Usage
Deploy this smart contract to the SUI blockchain.
Interact with the contract through supported blockchain interfaces, providing necessary parameters for minting, combining, withdrawing, and burning NFTs.
