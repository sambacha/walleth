[![WallETH](https://raw.githubusercontent.com/walleth/walleth/master/app/src/main/res/mipmap-xhdpi/ic_launcher.png)](https://walleth.org)

[![on Google Play](https://ligi.de/img/play_badge.png)](https://play.google.com/store/apps/details?id=org.walleth)
[![on FDroid](https://ligi.de/img/fdroid_badge.png)](https://f-droid.org/repository/browse/?fdid=org.walleth)

## Besu Walleth

[WIP] Besu - see: https://github.com/sambacha/walleth/commit/974784e9a66e153c89fba21f688c69fa6a210c30

Issues: Not IBFT2 Compatible, see 

https://github.com/sambacha/walleth/blob/73eb26330ad72983b403095f160db5b7d73e0e6e/app/schemas/org.walleth.data.AppDatabase/2.json#L146

https://github.com/sambacha/walleth/blob/73eb26330ad72983b403095f160db5b7d73e0e6e/app/schemas/org.walleth.data.AppDatabase/2.json#L192



https://sourcegraph.com/github.com/sambacha/walleth/-/commit/50ba271059c9024910128f1d763d23633b396342#diff-cfeee7dd7a6626a9d40b82eaf3c86797R192

```

        "createSql": "CREATE TABLE IF NOT EXISTS `${TABLE_NAME}` (`hash` TEXT NOT NULL, `extraIncomingAffectedAddress` TEXT, `chain` TEXT, `creationEpochSecond` INTEGER, `from` TEXT, `gasLimit` TEXT NOT NULL, `gasPrice` TEXT NOT NULL, `input` TEXT NOT NULL, `nonce` TEXT, `to` TEXT, `txHash` TEXT, `value` TEXT NOT NULL, `r` TEXT, `s` TEXT, `v` INTEGER, `needsSigningConfirmation` INTEGER NOT NULL, `source` TEXT NOT NULL, `relayed` TEXT NOT NULL, `eventLog` TEXT, `isPending` INTEGER NOT NULL, `error` TEXT, PRIMARY KEY(`hash`))",

```

```
          {
            "fieldPath": "extraIncomingAffectedAddress",
            "columnName": "extraIncomingAffectedAddress",
            "affinity": "TEXT",
            "notNull": false
          },

```


WallΞTH
=======

Native Android Ethereum wallet.

Features
========


 - Networks main, görli, rinkeby, ropsten, kovan, POA, sokol, ETC, xDAI
 - Keys on your device under your control
 - Tokens (your own ERC-20 compatible or predefined like DAI, Unicorn, OMG, SNT, ZRC, GNO, ..)
 - Day/Night mode
 - ERC-67 / ERC-681 URLs (e.g. scanned from QR-Code)
 - ERC-55 Checksums
 - WalletConnect (https://walletconnect.org) 1.0 Support
 - Offline signing (compatible to Parity signing flow)
 - Testnets with direct link to faucets (on görli and ropsten even auto-fill of address)
 - JSON UTC key import/export
 - display value in fiat like EUR, NZD, USD, .. or MakerDAO DAI
 - display function calls when available from https://github.com/ethereum-lists/4bytes
 - TREZOR (https://trezor.io) Support via USB-OTG - model 1 (v1.8.X) and model T (v2.1.X) are supported
 - KeyCard (https://keycard.status.im) support
 - watch only accounts
 - one flavor contains go-ethereum light client

find more information on https://walleth.org

References
==========

* [ERC67](https://github.com/ethereum/EIPs/issues/67)
* [ERC681](https://eips.ethereum.org/EIPS/eip-681)
* [ERC20](https://eips.ethereum.org/EIPS/eip-20)
* [Import Geth - a Devcon2 talk](https://ethereum.karalabe.com/talks/2016-devcon.html#1)
* [go Mobile:-Account-management](https://github.com/ethereum/go-ethereum/wiki/Mobile:-Account-management)
* [Ethereum visual reference](https://www.ethereum.org/images/logos/Ethereum_Visual_Identity_1.0.0.pdf)

License
=======

GPL
