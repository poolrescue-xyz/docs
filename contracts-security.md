---
icon: shield
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Contracts & Security

## Contracts & Security

PoolRescue is a non-custodial recovery tool — it never takes ownership of user assets.\
All interactions happen directly between the connected wallet and the target protocol’s contracts.\
The PoolRescue contracts serve only as minimal automation helpers and routing logic.

***

#### 🧩 Deployment Overview

All PoolRescue contracts are open-source and published in the [GitHub repository.](https://github.com/poolrescue-xyz/contracts)\
They are verified on the corresponding chain explorers.

<table><thead><tr><th width="110.428466796875">Chain</th><th width="80.8568115234375">Chain ID</th><th width="378.8565673828125">Contract</th><th>Explorer</th></tr></thead><tbody><tr><td><strong>Arbitrum</strong></td><td>42161</td><td><code>0x35c7477d8309ab3cfe869b863c939a47c651a6cd</code></td><td><a href="https://arbiscan.io/address/0x35c7477d8309ab3cfe869b863c939a47c651a6cd">arbiscan.io</a></td></tr><tr><td><strong>Arbitrum Nova</strong></td><td>42170</td><td><code>0xdfa523d19c244a9ac454e0f98b3dab6d53ac1cf1</code></td><td><a href="https://nova.arbiscan.io/address/0xdfa523d19c244a9ac454e0f98b3dab6d53ac1cf1">nova.arbiscan.io</a></td></tr><tr><td><strong>Avalanche</strong></td><td>43114</td><td><code>0xEbbA328cbCb051eBc89d7C47955264047e32D711</code></td><td><a href="https://snowscan.xyz/address/0xa0cf7113fcf9a1edfe0e59e7856148705cc9e245">snowscan.xyz</a></td></tr><tr><td><strong>Base</strong></td><td>8453</td><td><code>0x02f573bffb6728bdd3eb94f4808579b726d010eb</code></td><td><a href="https://basescan.org/address/0x02f573bffb6728bdd3eb94f4808579b726d010eb">basescan.org</a></td></tr><tr><td><strong>BNB Chain</strong></td><td>56</td><td><code>0x7c2da50ced123c85bea6b74c58ffb2f6d5a8d8ed</code></td><td><a href="https://bscscan.com/address/0x7c2da50ced123c85bea6b74c58ffb2f6d5a8d8ed">bscscan.com</a></td></tr><tr><td><strong>Ethereum</strong></td><td>1</td><td><code>0xba8b97a6afbc624b460fe88707fa8e3892155dce</code></td><td><a href="https://etherscan.io/address/0xba8b97a6afbc624b460fe88707fa8e3892155dce">etherscan.io</a></td></tr><tr><td><strong>Linea</strong></td><td>59144</td><td><code>0x02f573bffb6728bdd3eb94f4808579b726d010eb</code></td><td><a href="https://lineascan.build/address/0x02f573bffb6728bdd3eb94f4808579b726d010eb">lineascan.build</a></td></tr><tr><td><strong>Mantle</strong></td><td>5000</td><td><code>0xa0cf7113fcf9a1edfe0e59e7856148705cc9e245</code></td><td><a href="https://mantlescan.xyz/address/0xa0cf7113fcf9a1edfe0e59e7856148705cc9e245">mantlescan.xyz</a></td></tr><tr><td><strong>opBNB</strong></td><td>204</td><td><code>0xd8ac51dfbbc457f72669b2bbdf438544b2431b</code></td><td><a href="https://opbnb.bscscan.com/address/0xd8ac51dfbbc457f72669b2bbdf438544b2431b65">opbnb.bscscan.com</a></td></tr><tr><td><strong>Optimism</strong></td><td>10</td><td><code>0x1cf49a55dc5c07085b0b08130ee408a5fb94eb77</code></td><td><a href="https://optimistic.etherscan.io/address/0x1cf49a55dc5c07085b0b08130ee408a5fb94eb77">optimistic.etherscan.io</a></td></tr><tr><td><strong>Polygon</strong></td><td>137</td><td><code>0xa7816b5a6ba74032d7608351d115534359a0c0b2</code></td><td><a href="https://polygonscan.com/address/0xa7816b5a6ba74032d7608351d115534359a0c0b2">polygonscan.com</a></td></tr><tr><td><strong>Scroll</strong></td><td>534352</td><td><code>0xd4ef4d2c69af65f5c20b4b920cae71851066fed6</code></td><td><a href="https://scrollscan.com/address/0xd4ef4d2c69af65f5c20b4b920cae71851066fed6">scrollscan.com</a></td></tr><tr><td><strong>zkSync Era</strong></td><td>324</td><td><code>0xe11c2689cde43382d7f595b77bbef73f3a1c124b</code></td><td><a href="https://era.zksync.network/address/0xE11C2689cDE43382D7F595b77BBEf73F3A1c124b">era.zksync.netwrotk</a></td></tr></tbody></table>

***

#### 🧠 Security Philosophy

PoolRescue was built around **simplicity and transparency** — the contract logic is minimal by design:

* No asset custody, staking, or wrapping.
* No user data stored on servers.
* No admin keys or upgradeable proxies.
* Open-source verification on GitHub for every deployed version.

Developers and community members are encouraged to review and replicate the contracts directly from source.

***

#### 💸 Fee Logic

During the alpha phase, PoolRescue applies a **2.5% fee on recovered tokens**.\
This small fee supports ongoing infrastructure and maintenance, including:

* RPC endpoints and node providers
* Frontend hosting and domain costs

The fee is automatically deducted at execution

***

#### 🧾 Transparency

* 📂 **Source Code:** [GitHub – PoolRescue](https://github.com/Stakeridoo/PoolRescue)
* 🌐 **App:** [poolrescue.xyz](https://www.poolrescue.xyz)

