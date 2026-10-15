<div align="center">

# THRUSTCHAIN · DeltaV THRUST

**A modular multistage launch vehicle on BNB Smart Chain. 22,000 THRUST = 1 CLAIM.**

[deltavthrust.com](https://deltavthrust.com) · [THRUST.oracle](https://deltavthrust.com/price) · [Cockpit](https://deltavthrust.com/cockpit) · [Buy $50 with USDC](https://pancakeswap.finance/swap?chain=bsc&inputCurrency=0x8AC76a51cc950d9822D68b83fE1Ad97B32Cd580d&outputCurrency=0x969F60Bfe17962E0f061B434596545C7b6Cd6Fc4&exactField=input&exactAmount=50)

</div>

---

## The cockpit

You enter through **[login333](https://deltavthrust.com/login333)**, the airlock: one wallet signature, no transaction,
no gas. The **[cockpit](https://deltavthrust.com/cockpit)** is the view from the nose tip.

| seat | what opens |
|---|---|
| **Visitor** | the deck, every pool and THRUST.oracle |
| **Signed in** | your seat: THRUST stats, your THRUST, sending it |
| **Holder** | the holder deck |
| **VIP (22,000+ THRUST)** | your own ship ([/ship](https://deltavthrust.com/ship)), the lounge, the DAIO panel and the THRUSTfund locker |

Every transaction is built by the page and signed in your own wallet. The pages hold no key.

## deltavthrust.com

| page | |
|---|---|
| [/](https://deltavthrust.com) | the launch pad: price in USDC, market cap, liquidity, the lock, the rebase backlog |
| [/price](https://deltavthrust.com/price) | **THRUST.oracle**: every THRUST pair read at one block, priced from reserves, exact to 18 decimals. Live: xTHRUST readings on Injective and Arbitrum (reserved until a pool exists) and on Zilliqa EVM (planned, over the PULSAR peg), with each chain's own coin price checked against BSC |
| [/chart](https://deltavthrust.com/chart) | price history, every pool, liquidity and locks |
| [/cockpit](https://deltavthrust.com/cockpit) | the cockpit (above) |
| [/narrative](https://deltavthrust.com/narrative) | THRUST.narrative: Captain Demiurge's flight plan |
| [/bridge](https://deltavthrust.com/bridge) | the THRUST Bridge |
| [/data/thrust-pairs.json](https://deltavthrust.com/data/thrust-pairs.json) | the THRUST.oracle feed: public, readable from any origin, refreshed every 5 minutes |

- **Mirror:** [thrust.pythai.net](https://thrust.pythai.net).
- **Releases:** v1.2.6 is live on deltavthrust.com. The cockpit is a console: a main display that expands to fill the canopy, a price banner (Bitcoin, ETH, BNB, THRUST, BLAST, INJ, 0G; on/off), the helm, a services lounge with an open berth, and COMMS headlines. Built behind the sealed sign-in, opening when the login perspective is delivered: boarding and the pilot's seat (top up to VIP), the price board for every signed-in pilot, the chart and trade ($50 USDC and the 1,000,000 THRUST maximum buy) below 22,000 THRUST, and for VIP holders the THRUST Bridge route planner on chainmarketcap. /bridge shows the fee schedule and the VIP fee. IPFS copy `bafybeig6xjrqrw22de7z4adgdlfdyxmorevonqsfnbfnb5pmuiasbw7t3e`; DNSLink is not set yet.
- **IPFS:** the publishing flow is built: each release will be pinned as CIDv1, opened through
  `https://<cid>.ipfs.inbrowser.link/`, and named by the DNSLink record `_dnslink.deltavthrust.com`. No release has
  been published to IPFS yet, and the DNSLink record is not set.
- **Arweave:** the same bundle is built for the permaweb. It is not uploaded yet.

## The token: DeltaV THRUST

| | |
|---|---|
| **Contract** | [`0x969F60Bfe17962E0f061B434596545C7b6Cd6Fc4`](https://bscscan.com/token/0x969F60Bfe17962E0f061B434596545C7b6Cd6Fc4) (BSC, chain 56). Verified source `DeltaV.sol`, symbol THRUST, 18 decimals |
| **Launched** | 2022-04-03, block 16,633,406 |
| **Rebase** | Every transaction in a new second pays one owed step to every holder. Missed steps wait in the backlog; none are lost |
| **Fees** | 5% on buys and sells through a pool (1% liquidity, 3.5% treasury, 0.5% burn). Wallet-to-wallet transfers pay none |
| **Circulating supply** | total − dEaD − 0x0 (the contract's `getCirculatingSupply()`), every holder and every pair included |
| **Market cap** | circulating supply × the THRUST.oracle index |

### Wallets

| role | address |
|---|---|
| Owner | [`0xC75B704446D36d296C7138df969b4C1ba54D7326`](https://bscscan.com/address/0xC75B704446D36d296C7138df969b4C1ba54D7326) |
| Treasury (marketing, community, development) | [`0xa54B66632CFe3aD5C1520cB9a01666f0d76C79d4`](https://bscscan.com/address/0xa54B66632CFe3aD5C1520cB9a01666f0d76C79d4) |
| **PULSAR**: 2-of-3 Safe | [`0x34007ca21E12D1d31EAeA468f8f1639E6465508b`](https://bscscan.com/address/0x34007ca21E12D1d31EAeA468f8f1639E6465508b) |
| PULSAR triumvirate | `0x4bf8dBA345871BBC7A1E0ff41b7022D1770B3EB9` · `0xA414bA4Bd44C147249DA3428632fbf8f1e6D2f7b` · `0xd11baD2A987Eb9a43605c39f28Ff9eB338825104` |
| Burn | [`0x000000000000000000000000000000000000dEaD`](https://bscscan.com/token/0x969F60Bfe17962E0f061B434596545C7b6Cd6Fc4?a=0x000000000000000000000000000000000000dEaD) |

PULSAR collects its rebase and sends it to dEaD. It does not sell, because a 2-of-3 majority of the triumvirate will not
vote to sell.

### Liquidity pairs and locks (PancakeSwap v2, BSC)

| pair | address | the LP tokens |
|---|---|---|
| **THRUST / WBNB** (main pool) | [`0x8bee7bc7167bace12371ab5f87adb1f4212b2bc7`](https://bscscan.com/address/0x8bee7bc7167bace12371ab5f87adb1f4212b2bc7) | **83.3% in the [Mudra Locker](https://bscscan.com/address/0xAE7E6CAbad8d80f0b4E1C4DDE2a5dB7201eF1252)**; 16.6% with the owner |
| THRUST / BTCB | [`0x8988b9e8266c894297b6f2fd5597a8ecfdf49774`](https://bscscan.com/address/0x8988b9e8266c894297b6f2fd5597a8ecfdf49774) | owner |
| THRUST / ETH | [`0xf8ee40ee68024144df26f7162b2d1d8967e39f35`](https://bscscan.com/address/0xf8ee40ee68024144df26f7162b2d1d8967e39f35) | treasury |
| THRUST / USDC | [`0x762e1925cc37ac085dc81732113e0eb1382c4d2b`](https://bscscan.com/address/0x762e1925cc37ac085dc81732113e0eb1382c4d2b) | treasury |
| THRUST / ZIL | [`0xd7b52356e7cef48a3e2508c4a643d38f36cc67f3`](https://bscscan.com/address/0xd7b52356e7cef48a3e2508c4a643d38f36cc67f3) | treasury |

The Mudra Locker [`0xAE7E6CAbad8d80f0b4E1C4DDE2a5dB7201eF1252`](https://bscscan.com/address/0xAE7E6CAbad8d80f0b4E1C4DDE2a5dB7201eF1252)
holds three locks on the main pool:

| lock | share of the pool | term |
|---|---|---|
| **54859** | ≈ 56.7% | **locked to 2124-06-06**: the 100-year anchor |
| 55247, 55453 | ≈ 26.7% together | term ended 2025-06; the LP is still in the locker |

[/chart](https://deltavthrust.com/chart#dvx-locks) reads the current shares live. The other pairs' LP is the team's,
held by the owner and the treasury.

### Built, not deployed

These contracts have addresses reserved through create3d (factory `0xa5A2581d564248801cc5e06DbB764c99c170320A`). The
THRUST owner is the deployer. **Nothing is at these addresses yet. Do not send anything to them.**

| contract | reserved address | what it does |
|---|---|---|
| **ThrustDAIO** | `0xab68e5e68Ce944b0eAb17962F1285C2d392f8438` | the PULSAR triumvirate (2-of-3, 48 h timelock) with passenger signals (22,000 THRUST = 1 CLAIM, advisory) and the owner as guardian (veto only) |
| **ThrustVoteBox** | `0x3CCaF379776D09dBBD1E261894dB38a7C35F574f` | the ballot box for `contract.vote` on gas-conscious chains; on BNB, passengers vote by signature |
| **THRUSTfund** | `0x5275208BEb268409e7469944e406748dbA4Dca3a` | the timelock locker, extrapolated from LUVlocker |
| **ThrustAdapter** (xTHRUST, BSC) | `0xd7492003F82840D67d327B5C7f750a1Fe0932365` | locks THRUST when it leaves BSC and unlocks it when it comes home |
| **xTHRUST** (every landing chain) | `0x74EcB05660D9432434c79c68311d6f2A46D0ee72` | minted when THRUST is locked, burned when it goes home: Ethereum, Blast, 0G, Injective, Arbitrum |
| **PegPool** (Ethereum) | `0xCd89E5D79718140f5d8591b1ffdfc87e27d33493` | the bridge's own xTHRUST/WETH pool; the rebase on locked THRUST flows into it |
| **THRUSTswap V2 factory** (Injective) | `0x57f844018636CffaA5362F04f3d4fe62725f82eA` | the official Uniswap V2 build, unmodified (GPL-3.0-or-later), since Injective has no Uniswap; Arbitrum uses Uniswap V2 as it is |
| **THRUSTswap V2 router** (Injective) | `0x7B9D791b04964c3B625CEad48e6EE4E24BC9aFe0` | its router, paired with WINJ |

**xTHRUST** is token for token: Σ xTHRUST on every chain equals what the adapter has outstanding, and that never exceeds
the THRUST locked on BSC. PULSAR bridges like anyone else, with 2-of-3 signatures, and never sells. Before PULSAR receives
xTHRUST on a chain, its own safe is recreated there at the same address with the same three keys. Once wired, every
contract is sealed: no owner and no way to change the routes. The whole sequence has been rehearsed on local forks of
BSC, Ethereum, Blast, Injective and Arbitrum, including a direct Injective → Arbitrum transfer and THRUSTswap pools on
both. Nothing has been broadcast.

GOLDEN RATIO, StargateRelay and THRUSTbus are built and tested, and none is deployed. None of the new contracts has had
an external audit.

## Names: Unstoppable Domains

[deltavthrust.wallet](https://ud.me/deltavthrust.wallet) · [deltavthrust.crypto](https://ud.me/deltavthrust.crypto) ·
[deltavthrust.nft](https://ud.me/deltavthrust.nft) · [deltavthrust.zil](https://ud.me/deltavthrust.zil) ·
[deltavthrust.blockchain](https://ud.me/deltavthrust.blockchain) · [deltavthrust.dao](https://ud.me/deltavthrust.dao)

## Channels

| | |
|---|---|
| X | [@deltavexchange](https://x.com/deltavexchange) |
| Telegram | [t.me/deltavthrust](https://t.me/deltavthrust) |
| Medium | [deltavthrust.medium.com](https://deltavthrust.medium.com/) · [@deltaverse](https://medium.com/@deltaverse) |
| Markets | [GeckoTerminal](https://www.geckoterminal.com/bsc/pools/0x8bee7bc7167bace12371ab5f87adb1f4212b2bc7) · [BscScan](https://bscscan.com/token/0x969F60Bfe17962E0f061B434596545C7b6Cd6Fc4) · [PancakeSwap](https://pancakeswap.finance/swap?chain=bsc&inputCurrency=BNB&outputCurrency=0x969F60Bfe17962E0f061B434596545C7b6Cd6Fc4) |
| OpenSea | [thrusted](https://opensea.io/collection/thrusted) · [deltavthrust](https://opensea.io/collection/deltavthrust) |
| GitHub | [THRUSTDeltaV](https://github.com/THRUSTDeltaV) (the contract, DELTAVstargaterouter) · [thrustdrop](https://github.com/thrustdrop) (airdrop lab) · [DeltaVThrust-NFT](https://github.com/DeltaVThrust-NFT) (NFT source collection) |

## Repositories here

| repo | |
|---|---|
| **THRUST** | the project: THRUST.oracle, the cockpit, login333, ThrustDAIO, THRUSTfund, xTHRUST, the release gate. Private until after deployment |
| **THRUSTswap** | the DeltaV THRUST exchange, forked from the Uniswap interface (GPL-3.0). It lists xTHRUST on Arbitrum; Injective needs a chain entry the interface does not have yet. Private until after deployment |
| **thrustbridge** | ThrustBridge, the bridge mechanics: the Stargate V2 bridge interface, StargateRelay with the BANKON and VIP fees, and xTHRUST over LayerZero V2, with tests and deploy scripts. Private until deployment. |
| chain work | THRUST TNT: EVM chain research (subnet-evm, coreth, teleporter, Blast, Optimism and more) |

Related: [interplanetaryfilesystem](https://github.com/interplanetaryfilesystem) (the IPFS development archive that deltavthrust.com's
IPFS copy builds on) · [deltavchain](https://github.com/deltavchain) · [THCHAIN](https://github.com/THCHAIN)

## Security

Please report privately first: [Telegram](https://t.me/deltavthrust) or
[security.txt](https://deltavthrust.com/.well-known/security.txt).

---

<div align="center">

Nothing here is financial advice. Figures on deltavthrust.com are read live from the chain.

[deltavthrust.com](https://deltavthrust.com) · [Professor-Codephreak](https://github.com/Professor-Codephreak)

</div>
