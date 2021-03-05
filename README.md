Clockspeed
==========
one-CPU-one-vote, the world’s fastest PoW blockchain  
https://clockspeed-project.github.io


> **Abstract.** Clockspeed is the world's fastest PoW blockchain, that has the first Native SegWit (Bech32) built-in by default. Unlike Bitcoin, Clockspeed has no rounding errors when the block reward is halved. It launched fairly and follows Nakamoto's one-CPU-one-vote.


Introduction
------------
Clockspeed is a decentralized, peer-to-peer (P2P) digital currency and payment network supported by an open-source blockchain protocol, launched by Zenny Kim and Volodymyr Biloshytskyi on August 24, 2019 <sup>[[1]](#bitcointalk)</sup>. Through Clockspeed, users can make payments to anyone in the world at the highest speeds ***in 5 seconds***, and the lowest costs compared to other digital assets. For example, the transaction speed of Clockspeed is 120 times faster than Bitcoin, 30 times faster than Litecoin and 12 times faster than Dogecoin.

The Clockspeed Project emerged as an alternative solution to Bitcoin in light of early concerns over Bitcoin’s wait times in confirming block transactions and rounding errors in block reward halving. By introducing minor technical modifications to the original Bitcoin source code, Clockspeed allowed for much faster transaction speeds, even lower processing fees and has ***the most accurate block reward halving and total supply*** than any other digital asset, including Bitcoin. Clockspeed also launched following the ***one-CPU-one-vote*** idea proposed by Satoshi Nakamoto himself, thus making YespowerClock GPU and ASIC resistant. It has also launched as being the first blockchain to have ***Native SegWit (Bech32)*** enabled by default.

As one of the successful derivatives of Bitcoin, Clockspeed is establishing its position as ***the world's fastest PoW blockchain***, complementing and reinforcing Bitcoin in purpose, function, and utility, and challenging our traditional notions of money. The Clockspeed Project has ***never been funded through an ICO or premine***, making it a fair launch. Clockspeed is an entirely community and voluntarily driven project, with no external company or funding supporting it apart from community funding.

<small>** <a name="bitcointalk">[1]</a>: [Bitcointalk: [ANN] Clockspeed [CPU] Launching 2019/08/24 15:00 UTC](https://bitcointalk.org/index.php?topic=5177722.0)
</small>


Specifications
--------------
| | |
------------|------------
Block time: | `5` Seconds
Block reward: | `42.94967296` CLOCK
Halving interval: | `12,500,000` Blocks (approx. 2 years)
Total supply: | `1,073,741,824` CLOCK
PoW algorithm: | YespowerClock (based on Yespower 1.0.1)
Difficulty: | ClockShield-N510 (based on Zcash's modification of Digishield)
Port: | 5188 / RPC 34229
Premine: | None: NO ICO, NO Presale, NO Founder's rewards


The world's fastest PoW blockchain
----------------------------------
- 5 seconds transaction speed <sup>[[2]](#CLOCK_blocktime)</sup> :
  * 120x faster than Bitcoin
  * 30x faster than Litecoin
  * 12x faster than Dogecoin
- Transaction speed comparison
  <sup>[[3]](#DGB_blocktime)</sup>
  <sup>[[4]](#XVG_blocktime)</sup>
  <sup>[[5]](#DOGE_blocktime)</sup>
  <sup>[[6]](#LTC_blocktime)</sup>
  <sup>[[7]](#BTC_blocktime)</sup>
  <br>
  <img src="image/txspeed.png" width="95%">
  <br>
- Don't worry about orphan blocks:
  * According to the testnet results, the average orphan rate is under 3% and no problems occur.

<small>** <a name="CLOCK_blocktime">[2]</a>: [Github: CLOCK speed](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/chainparams.cpp#L187)
** <a name="DGB_blocktime">[3]</a>: [DGB speed](https://github.com/digibyte/digibyte/blob/82414be2e78bd136daeb91f55c72768a9b700957/src/chainparams.cpp#L88)
** <a name="XVG_blocktime">[4]</a>: [XVG speed](https://github.com/vergecurrency/verge/blob/4ae658a47ff3ea7af269cf408387e8265cccf197/src/chainparams.cpp#L85)
** <a name="DOGE_blocktime">[5]</a>: [DOGE speed](https://github.com/dogecoin/dogecoin/blob/0b46a40ed125d7bf4b5a485b91350bc8bdc48fc8/src/chainparams.cpp#L89)
** <a name="LTC_blocktime">[6]</a>: [LTC speed](https://github.com/litecoin-project/litecoin/blob/81c4f2d80fbd33d127ff9b31bf588e4925599d79/src/chainparams.cpp#L74)
** <a name="BTC_blocktime">[7]</a>: [BTC speed](https://github.com/bitcoin/bitcoin/blob/48c1083632687a42ac603d4f241e70616a1d3815/src/chainparams.cpp#L77)
</small>


Native SegWit (Bech32)
----------------------
- The first blockchain to have Native SegWit (Bech32) built-in by default.
- Significantly faster and lower cost than legacy transaction.
- Very high probability of detection guaranteed.
- Structure
  <sup>[[8]](#bip-0173)</sup>
  <sup>[[9]](#native_segwit-youtube)</sup>
  <sup>[[10]](#native_segwit-keynote)</sup>
  <br>
  <img src="image/bech32_structure.png" width="75%">
  <br>

<small>** <a name="bip-0173">[8]</a>: [Github: BIP-173](https://github.com/bitcoin/bips/blob/master/bip-0173.mediawiki)
** <a name="native_segwit-youtube">[9]</a>: [Youtube: New Address Type for SegWit Addresses by Pieter Wuille](https://www.youtube.com/watch?v=NqiN9VFE4CU)
** <a name="native_segwit-keynote">[10]</a>: [File: Keynote Document](https://prezi.com/gwnjkqjqjjbz/bech32-a-base32-address-format/)
</small>


Exact halving and total supply
------------------------------
Halving is everything about limiting the total supply. Bitcoin is valuable because its total supply has been strictly limited, unlike traditional currencies. This total supply is controlled only by that halving. There is nothing else. We made this halving better.
- The formula of Clockspeed’s total money supply (in satoshis)
  <sup>[[11]](#BTC_whitepaper)</sup>
  <sup>[[12]](#BTC_supply)</sup>
  <br>
  <img src="image/supply_formula.png" width="40%">
  <br>
- Block reward:
  * The block reward should be to a ***power of two***, so that it halves correctly.
  * `2^32/1e+8 = 42.94967296 CLOCK` <sup>[[13]](#CLOCK_blockreward)</sup>
- Halving schedule:
  * Interval `12500000 blocks (5^8*32)` <sup>[[14]](#CLOCK_halving_interval)</sup> which is approx. 2 years (62,500,000 seconds).
  * The total number of times halving will occur is 33 times, over the span of approx. 66 years (34,375,000 minutes).
- Total supply:
  * `1073741824 CLOCK` <sup>[[15]](#CLOCK_total_supply)</sup> <sup>[[16]](#CLOCK_total_cap)</sup> in theory, and `1073741823.875 CLOCK` <sup>[[17]](#CLOCK_total_test)</sup> <sup>[[18]](#CLOCK_total_test_qt)</sup> in actual.
  * The difference is `0.125 CLOCK`. One Satoshi (0.00000001) limitation makes this difference. In addition, this number is meaningful. FYI: `1 GB = 1073741824 Byte (2^30)`.
  * The total supply of Clockspeed is around 51 times greater than Bitcoin.
- Halving chart<br>
  ![halving_chart.png](https://raw.githubusercontent.com/clockspeed-project/clockspeed-project.github.io/master/image/halving_chart.png)
<!-- BEGIN - Hidden Halving table: -->
- <details><summary>Halving table <i>(click to expand)</i></summary><br>

  ![halving_table.png](https://raw.githubusercontent.com/clockspeed-project/clockspeed-project.github.io/master/image/halving_table.png)

  </details>
<!-- END - Hidden Halving table: -->

<small>** <a name="BTC_whitepaper">[11]</a>: [Bitcoin: A Peer-to-Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf)
** <a name="BTC_supply">[12]</a>: [Bitcoin Wiki: Controlled supply](https://en.bitcoin.it/wiki/Controlled_supply)
** <a name="CLOCK_blockreward">[13]</a>: [Github: Block Reward](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/validation.cpp#L1155)
** <a name="CLOCK_halving_interval">[14]</a>: [Halving Interval](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/chainparams.cpp#L135)
** <a name="CLOCK_total_supply">[15]</a>: [Total Supply](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/validation.cpp#L1147-L1216)
** <a name="CLOCK_total_cap">[16]</a>: [Total Cap](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/amount.h#L33)
** <a name="CLOCK_total_test">[17]</a>: [Total Test](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/test/main_tests.cpp#L48-L67)
** <a name="CLOCK_total_test_qt">[18]</a>: [Total Test(qt)](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/qt/test/paymentrequestdata.h#L437-L468)
</small>


one-CPU-one-vote
----------------
> “31/Oct/2008 Proof-of-work is essentially one-CPU-one-vote” <sup>[[11]](#BTC_whitepaper)</sup>

Satoshi Nakamoto talked about the importance of decentralized mining in his whitepaper. We want to create a blockchain that anyone can do mining easily without any entry barriers.
- CPU mining only
  * YespowerClock <sup>[[19]](#CLOCK_yespower_clock)</sup> (based on Yespower 1.0.1) is only for Clockspeed, not compatible with other Yespower coins.
  * The minimum difficulty (powlimit) is set low enough for two reasons. The first is to handle fast block time; The second is to allow mining on slow CPUs.
- Mining efficiency <sup>[[20]](#yespower)</sup> :
  * According to the test results, the most efficient is using ***half of threads*** on a single CPU.
  * YespowerClock is more suitable for older CPUs, because it is essentially a ***multi-threading resistor***. Suitable for smartphones and Raspberry Pi.
- Benchmark
  <br>
  <img src="image/yps_efficiency.png" width="90%">
  <br>
- NO GPU: GPU mining is not possible.
- NO ASIC: ASIC mining is not possible.

<small>** <a name="CLOCK_yespower_clock">[19]</a>: [Github: YespowerClock](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/primitives/block.cpp#L30-L70)
** <a name="yespower">[20]</a>: [Openwall: yespower - proof-of-work (PoW) scheme](https://www.openwall.com/yespower/)
</small>


Difficulty Adjustment Algorithm (DAA)
-------------------------------------
ClockShield-N510 is based on Zcash's modification of Digishield. Unlike the Zcash’s modification version, we use a moving average of `510 blocks (approx. 42.5 minutes)` <sup>[[21]](#CLOCK_clockshield_n510)</sup> <sup>[[22]](#CLOCK_clockshield_n510_pow)</sup>. To keep the block time 5 seconds, ClockShield-N510 adjusts the difficulty level.
- The formula of ClockShield-N510 <sup>[[23]](#zawy-digishield)</sup>
  ```bash
  t = timestamp, h = height,
  T = 5 (target block time in seconds),
  N = 510 (window size in blocks)
  ```
  <br>
  <img src="image/clockshield_formula.png" width="50%">
  <br>

- Block time vs difficulty at first launching on testnet<br>
  ![time_vs_difficulty.png](image/time_vs_difficulty.png)
  * It counts from block 1, an adjustment is made at block 511, and the actual control begins at block 512. [(log: time-diff)](https://raw.githubusercontent.com/clockspeed-project/clockspeed-project.github.io/master/log/time_vs_difficulty-13536.log)

- Nonce distribution at first launching on testnet<br>
  ![nonce_vs_difficulty.png](image/nonce_vs_difficulty.png)
  * The nonce is randomly well distributed. Difficulty changes but no bias. [(log: nonce-diff)](https://raw.githubusercontent.com/clockspeed-project/clockspeed-project.github.io/master/log/nonce_vs_difficulty-13548.log)

<small>** <a name="CLOCK_clockshield_n510">[21]</a>: [Github: ClockShield-N510](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/chainparams.cpp#L143-L170)
** <a name="CLOCK_clockshield_n510_pow">[22]</a>: [ClockShield-N510(pow)](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/pow.cpp)
** <a name="zawy-digishield">[23]</a>: [Summary of Difficulty Algorithms](https://github.com/zawy12/difficulty-algorithms/issues/50)
</small>


FAQ
---
- Disk space requirements:
  * Blockchain size growth is around `10 MB per day` and around 3.65 GB per year.
- Network rules:
  * To prevent fraud and timestamp attacks, nodes should be within `70 seconds` <sup>[[24]](#70_seconds)</sup> of accurate internet time, or they will be banned.
- Selfish mining & time warp attack:
  * Fraud techniques for manipulating timestamps are already known. We use a future time limit (FTL) to prevent this. Blocks that differ `60 seconds` <sup>[[25]](#FTL_60)</sup> or more from the current head will be banned. (credit: zawy12)
- Header indexing:
  * Using sha256d in header indexing, the initial synchronization speed is as fast as Litecoin.

<small>** <a name="70_seconds">[24]</a>: [Github: timedata.h](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/timedata.h#L23)
** <a name="FTL_60">[25]</a>: [Future Time Limit](https://github.com/clockspeed-project/clockspeed/blob/d2d13cacd9e7c2640a02e6392978a26df06f9eb8/src/chain.h#L36)
</small>


Wallet
------
[![Build Status](https://travis-ci.org/clockspeed-project/clockspeed.svg?branch=master-v0.16.3)](https://travis-ci.org/clockspeed-project/clockspeed)
![GitHub All Releases](https://img.shields.io/github/downloads/clockspeed-project/clockspeed/total)

Clockspeed’s first node software is called **Yumekawa (夢川)**. It can be translated in some ways.
- “Yume (夢)” means dream and “Kawa (川)” means river. So it’s *Dream River* in japanese.
- The second letter “Kawa” stands for “Kawaii (可愛い)”. In this case the meaning is *Dreamy Cute*.
- Also Yumekawa replaces the word ***Core*** (ie: Bitcoin Core). We think it sounds a bit centralized.

**Download**
- <img src="image/icon_win.png" width="18"> Win64: https://github.com/clockspeed-project/clockspeed/releases/latest
- <img src="image/icon_win.png" width="18"> Win32: https://github.com/clockspeed-project/clockspeed/releases/latest
- <img src="image/icon_linux.png" width="18"> Linux64 (x86_64): https://github.com/clockspeed-project/clockspeed/releases/latest
- <img src="image/icon_linux.png" width="18"> Linux32 (i686): https://github.com/clockspeed-project/clockspeed/releases/latest
- <img src="image/icon_osx.png" width="18"> OSX (Apple macOS): https://github.com/clockspeed-project/clockspeed/releases/latest
- <img src="image/icon_arm.png" width="18"> ARM64 (aarch64): https://github.com/clockspeed-project/clockspeed/releases/latest
- <img src="image/icon_arm.png" width="18"> ARM32 (arm): https://github.com/clockspeed-project/clockspeed/releases/latest
- Bootstrap: https://github.com/clockspeed-project/bootstrap/releases/latest
- Source: https://github.com/clockspeed-project/clockspeed


CPUMINER
--------
Native SegWit (Bech32) address is by default and strongly recommended. `-t1` uses 1 thread. If you want more hash, increase this number.

**cpuminer-opt-clockspeed (Win64 and Linux64)** ![GitHub All Releases](https://img.shields.io/github/downloads/cryptozeny/cpuminer-opt-clockspeed/total) : https://github.com/cryptozeny/cpuminer-opt-clockspeed/releases/latest

**clockmaker (BETA: All platforms)** ![GitHub All Releases](https://img.shields.io/github/downloads/decryp2kanon/clockmaker/total) : https://github.com/decryp2kanon/clockmaker/releases/latest
- Pool mining:
  ```bash
  ./cpuminer -a clockspeed -o stratum+tcp://1pool.clockspeed-project.github.io:3333 -u clock1qv0ahzfa2ssu47wes89390sl0jz6g05h0267u8g -t1
  ```
- Solo mining:
  * We strongly recommend solo mining for decentralization.
  * Make a file `clockspeed.conf`
    ```bash
    server=1
    rpcuser=username
    rpcpassword=password
    rpcallowip=127.0.0.1
    ```
  * Restart your Yumekawa wallet
  * Run cpuminer-opt-clockspeed (RPC=`34229`, testnet5 RPC=`44229`, regtest RPC=`45339`)
    ```bash
    ./cpuminer -a clockspeed -o http://localhost:34229 --no-longpoll -u username -p password --coinbase-addr=clock1qv0ahzfa2ssu47wes89390sl0jz6g05h0267u8g -t1
    ```
  * Detailed solo mining tutorials:
    - Windows: https://forum.clockspeed-project.github.io/d/9-solo-mining-on-windows
    - Linux: https://forum.clockspeed-project.github.io/d/20-solo-mining-on-linux


Pool
----
Please contact us if you have a new mining pool.
- 1pool@tokyo: https://1pool.clockspeed-project.github.io
- 2pool@tokyo: https://2pool.clockspeed-project.github.io
- rplant@worldwide: https://pool.rplant.xyz
- mofumofu@tokyo: https://nomp.mofumofu.me
- dxpool@china: https://www.dxpool.com
- anomp@china: http://anomp.com
- lepool@china: http://www.lepool.com.cn:8080
- nosuchpool@czechia: https://nosuchpool.cloud
- customspeed@netherlands: http://pool.customspeed.nl
- miningmadness@usa: https://www.miningmadness.com
- cpu-pool@russia: http://cpu-pool.com
- xpoolx@france: https://xpoolx.com
- nendly@usa: https://clock.nendly.com
- ~~zpool@worldwide: https://zpool.ca/algo/yespowerCLOCK~~ (Disabled)
- ~~zergpool@worldwide: https://zergpool.com/site/mining?algo=yespowerClock~~ (Disabled)
- bullcpupool@russia: http://bullcpupool.com
- reallypool@russia: http://reallypool.ru
- instapool@USA: https://instapool.xyz


Explorer
--------
- Iquidus: https://1explorer.clockspeed-project.github.io
- Addressindex: https://clock.wtf
- Addressindex (old stable): https://clockspeed-project.github.io/explorer
- Esplora: https://clock.wtf/esplora
- Esplora (old stable): https://clockspeed-project.github.io/esplora
- Verge: https://2explorer.clockspeed-project.github.io


Service
-------
- Node Map: https://map.okoto.xyz/clock
- Halving Counter: https://clockspeed-blockhalf.github.io
- API Addressindex: https://api.clockspeed-project.github.io
- Faucet: https://cpu-mining.info/clockspeed-faucet


3rd party wallet
----------------
- Android Wallet (Google Play Store): coming soon
- Android Wallet (APK download): https://github.com/clockspeed-project/android_wallet_clockspeed/releases/latest
- Web Wallet: https://clock.wtf/wallet
- Web Wallet (old stable): https://clockspeed-project.github.io/wallet
- Paper Wallet: https://nao20010128nao.github.io/WalletGenerator.net/?currency=clockspeed
- Paper Wallet (old stable): https://clockspeed-project.github.io/ClockWalletGenerator.net/?currency=clockspeed
- Wallet Extension for Google Chrome: https://chrome.google.com/webstore/detail/clockspeed-wallet-extensi/pgojdfajgcjjpjnbpfaelnpnjocakldb
- Wallet Extension for Firefox: https://addons.mozilla.org/en-US/firefox/addon/clockspeed-wallet-extension
- Tip Extension for Firefox: https://addons.mozilla.org/en-US/firefox/addon/clockgift


Testnet
-------
- Explorer Iquidus (testnet5): https://1explorer-testnet.cryptozeny.com
- Explorer Esplora (testnet5): https://clockspeed-project.github.io/esplora-testnet
- API Addressindex (testnet5): https://api-testnet.clockspeed-project.github.io
- Pool (testnet5): https://1pool-testnet.cryptozeny.com


Exchange
--------
- GX.COM
  * CLOCK-USDT: https://www.gx.com/trade/CLOCK_USDT
- ALTMARKETS.IO (v2)
  * CLOCK-BTC: https://v2.altmarkets.io/trading/clockbtc
- EX4ANGE.ORG
  * CLOCK-BTC: https://ex4ange.org/?CLOCK-BTC
  * CLOCK-DOGE: https://ex4ange.org/?CLOCK-DOGE
- OCCE.IO
  * CLOCK-BTC: https://www.occe.io/exchange/clock_btc
  * CLOCK-UAH: https://www.occe.io/exchange/clock_uah
- CEXZ.CA
  * CLOCK-LTC: https://www.cexz.ca/trading/clockltc
- ~~ALTILLY.COM~~ ***(Hacked 2020-12)***
  * ~~CLOCK-BTC: https://altilly.com/market/CLOCK_BTC~~
  * ~~CLOCK-DOGE: https://altilly.com/market/CLOCK_DOGE~~
  * ~~CLOCK-USDT: https://altilly.com/market/CLOCK_USDT~~
- ~~KUANGEX.COM~~ ***(Closed 2021-02)***
  * ~~CLOCK-USDT: https://www.kuangex.com/trade/clock_usdt~~
- ~~ALTMARKETS.IO (v1)~~ ***(Shutdown 2021-03)***
  * ~~CLOCK-BTC: https://altmarkets.io/trading/clockbtc~~
  * ~~CLOCK-DOGE: https://altmarkets.io/trading/clockdoge~~


Community
---------
- Telegram: https://t.me/clockspeed
- Twitter: https://twitter.com/clockspeed_dev
- Forum: https://forum.clockspeed-project.github.io
- Rocket.Chat: https://chat.clock.wtf
- Bitcointalk: https://bitcointalk.org/index.php?topic=5177722.0
- Reddit: https://www.reddit.com/r/Clockspeed


License
-------
Clockspeed Yumekawa is released under the terms of the MIT license. See [COPYING](https://github.com/clockspeed-project/clockspeed/blob/master-v0.16.3/COPYING) for more
information or see https://opensource.org/licenses/MIT.

- Copyright © 2009-2010 Satoshi Nakamoto
- Copyright © 2009-2018 The Bitcoin Core developers
- Copyright © 2013-2019 Alexander Peslyak - Yespower 1.0.1
- Copyright © 2016-2018 The Zcash developers - DigiShieldZEC
- Copyright © 2018-2020 The Clockspeed Yumekawa developers

