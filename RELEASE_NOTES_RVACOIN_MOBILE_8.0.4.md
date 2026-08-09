# RVACoin Mobile 8.0.4

This release provides a signed, non-debug Android build of RVACoin Mobile 8.0.4.

## Changes

- Fix message signing for wallets imported from legacy Bitcoin-version WIF private keys, resolving `Error Invalid network version`.
- Preserve RVACoin's current private-key network version for newly created and current-format wallets.
- Standardize the Android release asset name as `rvacoin-mobile.apk`.

## Build information

- Source: [RVACoin-io/rvacoin-mobile](https://github.com/RVACoin-io/rvacoin-mobile)
- Source commit: [`1fb365bb13a0bbe8c4bf5872b752159aee0b4aed`](https://github.com/RVACoin-io/rvacoin-mobile/commit/1fb365bb13a0bbe8c4bf5872b752159aee0b4aed)
- Android package: `io.bluewallet.bluewallet`
- Version code: `1786272238`
- Minimum Android API: 24 (Android 7.0)
- Build type: release (`debuggable=false`)
- Asset: `rvacoin-mobile.apk`
- Size: 82,460,789 bytes

## Signing certificate

The repository production signing secrets were not available to the build workflow. The APK is signed with the CI-generated temporary certificate below and verifies with Android APK Signature Schemes v2 and v3.

```text
DN: CN=Temp, O=BlueWallet, OU=CI, L=NY, ST=NY, C=US
Certificate SHA-256: d0d4a292f3aa020cb341bc17a70bc0e6f60eb429c301e07d7a5d2645e82d71e5
```

Android upgrades require the new APK to use the same signing certificate. A future build signed with a different certificate will require uninstalling this build first; back up wallet recovery information before uninstalling.

## Verify the download

SHA-256:

```text
76df86b0e70e6785be56a940a0109bbd8482c20263717b9ab86374600b1c26cb  rvacoin-mobile.apk
```

Only install the APK downloaded from this GitHub release or an official link published by RVACoin.
