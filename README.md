# Benchmarks

Codemagic released the powerful M2 Mac mini for the developers to build and test their apps faster. This document contains tests run on popular open-source native iOS projects to give you an idea about the fast speed in a real-world scenario and the comparison with M2 and M1 machines.

## [Xcode Benchmark](https://github.com/nevercode-rudrank/Benchmarks/tree/benchmark)

The first project is the famous `XcodeBenchmark` used to provide an idea about the performance of M1 Mac mini and Mac Pro. It is a framework that includes **42 popular CocoaPods** libraries and **70+ dependencies** in total.

**Test name** | **Codemagic (M2 Mac Mini)** | **Codemagic (M1 Mac Mini)**
--- | --- | ---
Running Benchmark Tests | **3m 35s** | 5m 35s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/Benchmarks/blob/benchmark/codemagic.yaml)

- Codemagic M2 Mac mini Workflow  [![Codemagic build status](https://api.codemagic.io/apps/6269b3cc6248df946a077233/ios-m2-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/6269b3cc6248df946a077233/build/643fb4210684b3b2706ae810) 
- Codemagic M1 Mac mini Workflow  [![Codemagic build status](https://api.codemagic.io/apps/6269b3cc6248df946a077233/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/6269b3cc6248df946a077233/build/643fb41cb7c6fae51e9d3a12) 

## [Wikipedia iOS](https://github.com/nevercode-rudrank/wikipedia-ios)

The official Wikipedia iOS app is open-sourced. It also contains multiple dependencies and hundreds of tests.

**Test name** | **Codemagic (M2 Mac Mini)** | **Codemagic (M1 Mac Mini)**
--- | --- | ---
Building Project | **1m 20s** | 1m 42s
Running Tests | **2m 34s** | 3m 27s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/codemagic.yaml)

- Codemagic M2 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/6267c85aeb4a9a0e7b7eba1b/wikipedia-m2-mini/status_badge.svg)](https://codemagic.io/app/6267c85aeb4a9a0e7b7eba1b/build/643fa4ada6c16df739a8e5c8)
- Codemagic M1 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/6267c85aeb4a9a0e7b7eba1b/wikipedia-m1-mini/status_badge.svg)](https://codemagic.io/app/6267c85aeb4a9a0e7b7eba1b/build/643fa4ada6c16df739a8e5c7)

## [Signal iOS](https://github.com/nevercode-rudrank/Signal-iOS)

Signal is a free, open source, messaging app for simple private communication with friends. It is a great project for testing out benchmarks that replicates a real-world application.

**Test name** | **Codemagic (M2 Mac Mini)** | **Codemagic (M1 Mac Mini)**
--- | --- | ---
Building and Testing | **6m 51s** | 7m 37s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/Signal-iOS/blob/main/codemagic.yaml)

- Codemagic M2 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/626e67f46248df64e0b79f91/ios-m2-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/626e67f46248df64e0b79f91/build/643fb05d4d88a8c286334f33)
- Codemagic M1 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/626e67f46248df64e0b79f91/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/626e67f46248df64e0b79f91/build/643fb0598854fcfe834a8b75)

## [Mastodon iOS](https://github.com/nevercode-rudrank/mastodon-ios)

The official Mastodon iOS app's repository is available as open-source.

**Test name** | **Codemagic (M2 Mac Mini)** | **Codemagic (M1 Mac Mini)**
--- | --- | ---
Building Project | **2m 12s** | 2m 50s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/mastodon-ios/blob/develop/codemagic.yaml)

- Codemagic M2 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/63a21b433246c3f84a9da7d4/mastodon-ios-m2/status_badge.svg)](https://codemagic.io/app/63a21b433246c3f84a9da7d4/build/643faf0fc112ac5cd5e19fb8)
- Codemagic M1 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/63a21b433246c3f84a9da7d4/mastodon-ios-m1/status_badge.svg)](https://codemagic.io/app/63a21b433246c3f84a9da7d4/build/643faf0fc112ac5cd5e19fb6)
