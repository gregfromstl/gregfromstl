# Bridging is Broken _(and how to fix it)_

Routing assets is the most critical piece to the rollup-centric roadmap. Without it, liquidity sits isolated on a single chain. With it, any given user can unlock the staggering diversity of thousands of EVM rollups.  Most of the focus thus far is on making bridges operational. We worry about speed, security, etc. and for good reason. But, we’re reaching a point where we should consider their optimal user experience. It’s time to refine how we route onchain assets into the experience developers and users expect.

Bridging speed, convenience, and reliability continue to improve for EVM rollups every day. You can visit any number of bridging sites and move your funds from one chain to another in a matter of seconds. But, bridges still stand isolated from the typical application experience. If a user wants to use an app on a new chain, they have to navigate to a dedicated site. Only after bridging their funds can they use the app they intended to in the first place. True multichain app UX includes “just-in-time” asset routing. The user doesn’t need to worry about bridges, chains, or anything besides the app they’re using. To reach such a user experience, there are a few barriers present in most modern bridges.

### Challenge 1: Expected Outputs
Many existing bridges use an input-first approach to bridge requests/intents. In these cases, users tell the bridge how much of the input asset they’re willing to pay. The bridge returns an output amount based on fees, slippage, dutch auction settlement, and other factors.

This protects the bridge or solvers from potential losses. When the output is flexible, the bridging/swapping process is easier to fulfill. Any number of things can cause the output to change up until the destination assets land in the user’s wallet. Slippage, fulfillment auctions, destination chain gas prices, and more can all contribute to increased costs to the user. By using an “expected” output amount, the bridge or solver isn’t liable for these costs. The user pays for any unexpected price increase through the decreased output.

As a user, this approach is problematic. When bridging funds, you’re often doing so with an intended action on the destination chain in mind. That action requires a certain number of funds to complete. If a user doesn’t know what amount they’ll receive, they’ll always have to send extra assets to account for any potential difference. This leaves those assets on the destination chain and isolated from your other funds. We’ve all experienced this with a “dusting” of various tokens across different chains.

_Note: One bridging provider (Relay), does allow for “exact output” routing. This is a 10X improvement on both developer and user experience. This isn’t easy though. Because most other bridges and DEXes don’t support anything like it, a lot more has to go into constructing those routes. All contracts or protocols should be designed with output-centric requests in mind._

### Challenge 2: Extra Fees
“Extra fees” are any required assets besides the ones you intend to use. Gas fees are the quintessential example of this, and smart account gas sponsorship has solved gas-related UX problems. But, gas sponsorship doesn’t apply to bridge fees.

Many bridges expect the destination gas or other fees in a token besides the one being bridged. This protects bridges and solvers from volatility in the token they’re bridging. By requesting any fees in a consistent asset such as ETH or USDC, the bridge or solver isn’t exposed to any price movements after providing a quote.

This convenience for the bridge becomes a severe inconvenience for users. If the user’s wallet doesn’t hold the expected fee asset, they’re not able to bridge at all! So, they need to swap some of their input asset to the requested fee asset. This adds inconvenience, cost, and friction to the user experience.

All bridges and DEXes need to quote their fees in the input token. Many do, but it needs to be a universal expectation and standard.

### Challenge 3: “One size fits all”
Over the past few years, countless bridging methods have attempted to solve the UX problems of the rollup-centric roadmap. Each one of these carries their own unique benefits and tradeoffs. It takes a combination of them to ensure complete asset and chain coverage across all EVM chains. Bridges today tend to focus on a single strategy, forcing developers to choose which tradeoffs to accept.

Intents are fast and inexpensive but solvers don’t operate on newer chains or handle lower liquidity tokens. Lock-and-mint contracts allow any token to exist anywhere but lead to wrapped token fragmentation. Native bridges are cost-effective, reliable, and available on all chains but are much slower. Each solution has its drawbacks, and picking one is settling for a limited feature set.

As an industry, we need unified interfaces for dealing with any asset router. App developers should be able to access any number of routing methods. The explosion of EVM rollups gave devs optionality under a single umbrella. It’s time we approach bridging the same way.

I’m aware of [ERC-7683](https://www.erc7683.org) and in many ways, this post is an indirect response to it. It misses (and even avoids) many of the true challenges of building multichain apps. At some point, I will write a more direct breakdown of that specific proposed standard.
