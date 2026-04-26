# Awesome TDLib [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of [TDLib](https://github.com/tdlib/td) bindings, wrappers, and tools.

[TDLib](https://core.telegram.org/tdlib) is Telegram's official cross-platform library for building Telegram clients. It handles network, encryption, and local storage, exposing a high-level API via `td_json_client` or native bindings.

This list focuses on **TDLib-based** projects. MTProto reimplementations (Telethon, Pyrogram, gramjs, MadelineProto, TLSharp, etc.) are out of scope — they speak the protocol directly without TDLib.

## Contents

- [Official](#official)
- [Bindings](#bindings)
- [Apps using TDLib](#apps-using-tdlib)
- [Build tooling](#build-tooling)
- [Resources](#resources)
- [Contributing](#contributing)

## Official

- [tdlib/td](https://github.com/tdlib/td) — Official TDLib repository. C++ source with native Java (JNI) and .NET (C++/CLI, C++/CX) bindings in tree.
- [TDLib documentation](https://core.telegram.org/tdlib) — Reference docs and getting-started guide.
- [td_api.tl](https://github.com/tdlib/td/blob/master/td/generate/scheme/td_api.tl) — Type Language schema describing every method and class. Most third-party bindings generate code from this file.
- [td_json_client](https://core.telegram.org/tdlib/docs/td__json__client_8h.html) — JSON interface description for language-agnostic integration.

## Bindings

### .NET / C#

- [egramtel/tdsharp](https://github.com/egramtel/tdsharp) — .NET Core bindings for TDLib.

### Dart

- [ivk1800/tdlib-dart](https://github.com/ivk1800/tdlib-dart) — Dart bindings generated from `td_api.tl`.

### Go

- [zelenin/go-tdlib](https://github.com/zelenin/go-tdlib) — Go wrapper for TDLib.

### Java / JVM

- [tdlight-team/tdlight-java](https://github.com/tdlight-team/tdlight-java) — Full Java client supporting both bots and userbots, based on TDLib.
- [TGX-Android/tdlib](https://github.com/TGX-Android/tdlib) — Prebuilt TDLib Java bundle used in Telegram X for Android.

### Kotlin Multiplatform

- [xephosbot/tdlib-kmp](https://github.com/xephosbot/tdlib-kmp) — TDLib Kotlin Multiplatform library.

### JavaScript / TypeScript (Node.js)

- [eilvelia/tdl](https://github.com/eilvelia/tdl) — Node.js bindings to TDLib.
- [airgram/airgram](https://github.com/airgram/airgram) — Strict-typed TS/JS library based on TDLib.

### Lua

- [giuseppeM99/tdlua](https://github.com/giuseppeM99/tdlua) — Lua interface to TDLib.

### PHP

- [thisismzm/tdlib-php-ffi](https://github.com/thisismzm/tdlib-php-ffi) — TDLib in PHP via the FFI extension.

### Python

- [pylakey/aiotdlib](https://github.com/pylakey/aiotdlib) — Asyncio Python client based on TDLib.

### React Native

- [vladlenskiy/react-native-tdlib](https://github.com/vladlenskiy/react-native-tdlib) — React Native wrapper for TDLib. Ships prebuilt binaries for iOS (xcframework) and Android (jniLibs); installation is `npm install` + autolink.

### Ruby

- [southbridgeio/tdlib-ruby](https://github.com/southbridgeio/tdlib-ruby) — Ruby bindings and client.

### Rust

- [antonio-antuan/rust-tdlib](https://github.com/antonio-antuan/rust-tdlib) — Rust client for TDLib.

### Swift / iOS / macOS

- [Swiftgram/TDLibKit](https://github.com/Swiftgram/TDLibKit) — Native Swift wrapper. Available on iOS, macOS, watchOS, tvOS, and visionOS.
- [Swiftgram/TDLibFramework](https://github.com/Swiftgram/TDLibFramework) — TDLib packaged as an XCFramework with Swift Package Manager support.

## Apps using TDLib

- [Unigram](https://github.com/UnigramDev/Unigram) — Open-source Telegram client for Windows.
- [Telegram X for Android](https://github.com/TGX-Android/Telegram-X) — Alternative Android client built on TDLib.

## Build tooling

- [xkaers/tdlib-build](https://github.com/xkaers/tdlib-build) — GitHub Actions to compile TDLib for Java/C# and any language using `td_json_client`.
- [tdlight-team/tdlight-java-natives](https://github.com/tdlight-team/tdlight-java-natives) — JNI native artifacts for tdlight-java per architecture and OS.
- [Sammers21/tdlib-java-builds](https://github.com/Sammers21/tdlib-java-builds) — GitHub Actions for building TDLib JNI bindings for Windows/macOS/Linux.

## Resources

- [td_json_client API](https://core.telegram.org/tdlib/docs/td__json__client_8h.html) — Reference for the JSON wire format.
- [TDLib methods](https://core.telegram.org/tdlib/docs/classtd_1_1td__api_1_1_function.html) — Auto-generated method list.
- [TDLib classes](https://core.telegram.org/tdlib/docs/classtd_1_1td__api_1_1_object.html) — Auto-generated class list.
- [Telegram API overview](https://core.telegram.org/api) — Where TDLib fits relative to Bot API and raw MTProto.

## Contributing

Pull requests welcome. To be included, an entry must:

- be a TDLib binding, wrapper, or tool — not an MTProto reimplementation (Telethon, Pyrogram, gramjs, MadelineProto, TLSharp speak the protocol directly and are tracked elsewhere);
- have a public source repository;
- be in a working state. Mark unmaintained projects with `(unmaintained)` in the description rather than removing them silently.

Open a PR adding the entry to the relevant alphabetically-ordered section. One entry per line in the format `- [owner/repo](url) — One-line description.`
