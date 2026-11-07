# Pet Food

How much did a wallet spend to keep its Fren Pets alive? Enter a wallet; the page shows what it paid the Fren Pet game on
Base in $FP (today's $IMD) and in ETH, what the tokens went to, how much of them the game burned, and what that is in dollars
right now.

`dist/` is the whole site: `index.html`, `icon.svg` and `data/` (the sums per wallet in 257 static files, a snapshot of the
chain up to Base block 54,364,854). The page reads only its own files and, for the prices, public Base RPCs: the token's Uniswap v2
pool and Chainlink's ETH/USD feed. No wallet connection, no analytics, nothing is signed.

Counted: tokens a wallet paid to the game that cannot come back (the V1 contract's mints and items; the V2 diamond's feeding,
shields, insurance, mints net of their refund, the 2023/24 treasury fee, accessories net of what was sold back, dice net of
winnings), and the ETH a player paid for loot boxes, passes, mints and items. Shown apart and not counted: upgrades and stakes (they
vest back, and a kill pays the rest to the pet's holder), pool swaps, refunds, and the rewards the game paid out.

Generated from the private source at `banse/aidude` `tools/frenpet` commit `35d6dfacdb0a` (see `build.json`). A fan page, not
affiliated with Fren Pet; the pixel pets and colours come from the Fren Pet brand pack (docs.pet.game, Branding).
