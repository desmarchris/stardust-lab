# Stardust Roadshow Lab

## Creating a Stardust Account
1. Go to https://dashboard.stardust.gg/
2. Create an email/password login, or connect with Discord/Google
3. Log in using your account landing on the home page of the dashboard
(Note, if you see an error like `Email already in use`, you probably already have an account with that email using a different login method. If you see this trying to login with google, you probably have an email/password account already created with that email)

## Create a game
1. Click `Add game`
2. Give a name, description, optional image, and choose a blockchain. You can pick between IMX, Solana and Polygon. For this lab, please use Polygon (mainnet) as we will use polygonscan in a later step
<img width="1512" alt="Screen Shot 2022-09-16 at 12 58 01 PM" src="https://user-images.githubusercontent.com/23266037/190690760-e9529208-cb56-4c14-a25d-74e65ee5d643.png">
3. Click `Confirm`
4. Find the tile for your newly create game and click `Select`


You've now provisioned a Stardust game on chain!

## Template
A template is an item type definition for your game. You must mint tokens from a previously created template. Examples of templates can be a camoflauge skin, resources like dirt, or categories of NFTs that you'll later mint.
1. In the left nav, click `Templates`
<img width="1512" alt="Screen Shot 2022-09-16 at 12 59 29 PM" src="https://user-images.githubusercontent.com/23266037/190691086-f0aeb5e1-317f-4425-ac65-278d44f69eb7.png">
2. Click `Add template`
3. Give a name, description, image, and supply cap
4. Select `NFT`
5. Add a custom property. This will create a metadata property on _all_ NFTs minted from this template
<img width="1512" alt="Screen Shot 2022-09-16 at 1 01 28 PM" src="https://user-images.githubusercontent.com/23266037/190691328-70e9e988-e439-4774-890d-062658f57c8d.png">
6. Create the template!

## Player / Wallet Creation
A player in Stardust refers to a given user's custodial wallet. All you need to create a player is a unique ID, and we will return a player ID to reference them later in Stardust.
1. In the left nav, click `Players`
<img width="1512" alt="Screen Shot 2022-09-16 at 1 02 05 PM" src="https://user-images.githubusercontent.com/23266037/190691463-0afc0640-7bbb-4ddf-9e83-13a5c82a9847.png">
2. Click `Add player`
3. Give a unique ID. This is typically an email address but can be anything you want
4. Add a custom property for Stardust to store about this user. This is optional. Add VIP as the name, change the type to `boolean`, and select `True`.
<img width="1512" alt="Screen Shot 2022-09-16 at 1 03 40 PM" src="https://user-images.githubusercontent.com/23266037/190691673-26c0ed3f-8ee1-47c7-a04c-41a8ad490506.png">
5. Click `Confirm` to create the player
6. Open the player by clicking `View details` on the new tile

From this page, you can see the player's inventory (empty right now), their ID, wallet address, and custom properties created about this player.

## Minting a token
1. Within the newly created player's info page, scroll down to the `Inventory` section
2. Click `Add` in the upper right of this box
<img width="1512" alt="Screen Shot 2022-09-16 at 1 11 48 PM" src="https://user-images.githubusercontent.com/23266037/190692935-33f11483-c523-46ae-9d4e-6ac86f533dd9.png">
3. Select the template that was created earlier
4. You can now add properties specific to the token / NFT that this player will create. It will inherit the property we added earlier to the template and append token specific properties you add now
<img width="1512" alt="Screen Shot 2022-09-16 at 1 12 42 PM" src="https://user-images.githubusercontent.com/23266037/190693030-4b7e9971-0fd4-499e-9ba1-e14f8cec53d1.png">
5. Click confirm!

Congrats, you've now minted a token on-chain! You should now see the item in this player's inventory, and can view the Token ID. 

## Viewing the token on Polygonscan
1. To view this token on polygonscan, first copy the `Wallet Address` in the upper left of the player's info page underneath their image and player ID
<img width="1512" alt="Screen Shot 2022-09-16 at 1 13 30 PM" src="https://user-images.githubusercontent.com/23266037/190693215-078378b6-8ee5-4833-a689-0f546b27f676.png">
2. Go to https://polygonscan.com/
3. Paste the address in the search bar
4. Tab over to `ERC-1155 Txns`
<img width="1512" alt="Screen Shot 2022-09-16 at 1 14 07 PM" src="https://user-images.githubusercontent.com/23266037/190693322-539b245f-f095-473b-9669-c52961470ff3.png">
5. You should then see a transaction showing the mint! This `Token ID` will match the Stardust `Token ID`.
<img width="1512" alt="Screen Shot 2022-09-16 at 1 14 44 PM" src="https://user-images.githubusercontent.com/23266037/190693374-4dc9601c-f303-41d6-bbf8-72b3a64739f2.png">
