# Stardust Roadshow Lab

## Creating a Stardust Account
1. Go to https://dashboard.stardust.gg/
2. Create an email/password login, or connect with Discord/Google
3. Log in using your account landing on the home page of the dashboard
(Note, if you see an error like `Email already in use`, you probably already have an account with that email using a different login method. If you see this trying to login with google, you probably have an email/password account already created with that email)

## Create a game
1. Click `Add game`
2. Give a name, description, optional image, and choose a blockchain. You can pick between IMX, Solana and Polygon. For this lab, please use Polygon (mainnet) as we will use polygonscan in a later step
3. Click `Confirm`
4. Find the tile for your newly create game and click `Select`

You've now provisioned a Stardust game on chain!

## Template
A template is an item type definition for your game. You must mint tokens from a previously created template. Examples of templates can be a camoflauge skin, resources like dirt, or categories of NFTs that you'll later mint.
1. In the left nav, click `Templates`
2. Click `Add template`
3. Give a name, description, image, and supply cap
4. Select `NFT`
5. Add a custom property. This will create a metadata property on _all_ NFTs minted from this template
6. Create the template!

## Player / Wallet Creation
A player in Stardust refers to a given user's custodial wallet. All you need to create a player is a unique ID, and we will return a player ID to reference them later in Stardust.
1. In the left nav, click `Players`
2. Click `Add player`
3. Give a unique ID. This is typically an email address but can be anything you want
4. Add a custom property for Stardust to store about this user. This is optional. Add VIP as the name, change the type to `boolean`, and select `True`.
5. Click `Confirm` to create the player
6. Open the player by clicking `View details` on the new tile

From this page, you can see the player's inventory (empty right now), their ID, wallet address, and custom properties created about this player.

## Minting a token
1. Within the newly created player's info page, scroll down to the `Inventory` section
2. Click `Add` in the upper right of this box
3. Select the template that was created earlier
4. You can now add properties specific to the token / NFT that this player will create. It will inherit the property we added earlier to the template and append token specific properties you add now
5. Click confirm!

Congrats, you've now minted a token on-chain! You should now see the item in this player's inventory, and can view the Token ID. 

## Viewing the token on Polygonscan
1. To view this token on polygonscan, first copy the `Wallet Address` in the upper left of the player's info page underneath their image and player ID
2. Go to https://polygonscan.com/
3. Paste the address in the search bar
4. Tab over to `ERC-1155 Txns`
