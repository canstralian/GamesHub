# SteamClient Redeem (gameshub.official.redeem.steamclient)

## Description
This plugin redeems Steam free games using the [py-steam](https://github.com/rfht/py-steam) library (a fork of [ValvePython/steam](https://github.com/ValvePython/steam) with protobuf 4.x/5.x compatibility).

If the secrets are not provided, the plugin will ask for manual input for 2fa code if required.

## [Requirements](requirements.txt)

### Security Note
This plugin uses the [rfht/py-steam](https://github.com/rfht/py-steam) fork instead of the official `steam` package to address a critical protobuf vulnerability (CVE-2025-4565 / SNYK-PYTHON-PROTOBUF-10364902). The official `steam[client]` package requires `protobuf~=3.0`, which conflicts with the security requirement for `protobuf>=4.25.8`. The rfht fork maintains full API compatibility while supporting newer protobuf versions.

## FAQ
- **How to get steam secrets?**  
Please refer to [this](https://github.com/JustArchiNET/ArchiSteamFarm/wiki/Two-factor-authentication#android-phone)

## Changelog
v1.0.0
- Initial release
