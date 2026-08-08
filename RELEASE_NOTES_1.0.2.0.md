# RVACoin Core 1.0.2.0

RVACoin Core 1.0.2.0 extends RVA Namespace authorization consistently across the desktop wallet and wallet RPC interface.

## Highlights

- Checks `allowed.txt`, then `allowed1.txt`, `allowed2.txt`, and subsequent non-empty lists in order.
- Accepts comma-separated and whitespace-separated authorization addresses.
- Uses the wallet's `m/0'/0'/0'` receiving address for authorization.
- Provides the authorization address and `rva-auth-requests@rvacoin.io` request instructions when access is denied.
- Adds daemon/CLI RPC commands `generatemnemonic` and `validatemnemonic` for 12-word BIP39 mnemonics.
- Includes Qt, daemon, CLI, and transaction utility builds for Windows and Linux.

The `rvacoin-tx` utility does not load a wallet or access the network, so wallet authorization and mnemonic RPC commands do not apply to it.

Only executable files are attached to this mirror release. Full platform packages and source archives are published in the main [RVACoin Core repository](https://github.com/RVACoin-io/rvacoin/releases/tag/v1.0.2.0).

## SHA-256 checksums

```text
c3356f439ca0a2f2028196f7e7e450f43c20cf077bd75648687a7a0b76538a76  rvacoin-cli-1.0.2.0-linux-x86_64
f9d957b287f2b44d15bce73c3f5dc1c5d1ca3d0dcbdfdbc170fce795e3ba43e3  rvacoin-cli-1.0.2.0-windows-x86_64.exe
4ee8c4d0b867ad5c78bf625992ea99caab932d6e20636c7088b6285b1db7c1db  rvacoin-qt-1.0.2.0-linux-x86_64
dc769643cbb5d7dc98c3025af042c8e8d7adf5cc64622d0603167ddf15d67645  rvacoin-qt-1.0.2.0-windows-x86_64.exe
32fef3119681aa16100226d206d235bbc80c628da877c22254727f66a07cb304  rvacoin-tx-1.0.2.0-linux-x86_64
6772ab38fafda7c9749896e394400be2cc6c6cf6105b85569e673b068db00947  rvacoin-tx-1.0.2.0-windows-x86_64.exe
2a5109bd699d11c2de8d4245e0006bd3f155546d8d552b6bb9ca7c4154d4931e  rvacoind-1.0.2.0-linux-x86_64
5c7cd4ebcd3ca7570f93e9b85c04807efffec8adf61d436b9afd641403909c2c  rvacoind-1.0.2.0-windows-x86_64.exe
```
