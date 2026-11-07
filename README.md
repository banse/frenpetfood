# Pet Food

How much did a wallet spend to keep its Fren Pets alive? Enter a wallet; the page shows what it paid the Fren Pet game on
Base in $FP (today's $IMD), what the tokens went to, how much of them the game burned, and what that is in dollars right now.

`dist/` is the whole site: `index.html`, `icon.svg` and `data/` (the sums per wallet in 257 static files, a snapshot of the
chain up to Base block 54,077,883). The page reads only its own files and, for the price, public Base RPCs: the token's Uniswap v2 pool
and Chainlink's ETH/USD feed. No wallet connection, no analytics, nothing is signed.

Counted: tokens a wallet paid to the game that cannot come back (the V1 contract's mints and items, the V2 diamond's feeding, shields,
insurance, mints, accessories net of what was sold back, dice net of winnings). Shown apart and not counted: upgrades and stakes,
pool swaps, refunds, and the $FP the game bought and burned for actions paid in ETH.

Generated from the private source at `banse/aidude` `tools/frenpet` commit `e6b91728a146` (see `build.json`). A fan page, not
affiliated with Fren Pet; the pixel pets and colours come from the Fren Pet brand pack (docs.pet.game, Branding).
