# Benchmarks

Codemagic released the powerful M1 Mac mini for the developers to build and test their apps faster. This document contains tests run on popular open-source native iOS projects to give you an idea about the fast speed in a real-world scenario and the comparison with Bitrise and GitHub Actions.

> The build times are subjective and depend on external factors like the network speed for fetching resources, project size, external third-party dependencies, number of tests, etc.

## [Xcode Benchmark](https://github.com/nevercode-rudrank/Benchmarks/tree/benchmark)

The first project is the famous `XcodeBenchmark` used to provide an idea about the performance of M1 Mac mini and Mac Pro. It is a framework that includes **42 popular CocoaPods** libraries and **70+ dependencies** in total.

**Test name** | **Codemagic** | **Bitrise** | **GitHub Actions**
--- | --- | --- | ---
Running Benchmark Tests | **2m 49s** | 2m 16s | 11m 29s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/Benchmarks/blob/benchmark/codemagic.yaml)
- [`bitrise.yml`](https://github.com/nevercode-rudrank/Benchmarks/blob/benchmark/bitrise.yml)
- [`github action ios.yml`](https://github.com/nevercode-rudrank/Benchmarks/blob/master/.github/workflows/ios.yml)

- Codemagic M1 Mac mini Workflow  [![Codemagic build status](https://api.codemagic.io/apps//636384f636dd120e8bce1532/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/636384f636dd120e8bce1532/build/63e3050e34df01f41f9f1db1) 
- Bitrise M1 Elite XL Workflow [![Build Status](https://app.bitrise.io/app/3352aa05cfe2f537/status.svg?token=kSu7Wj2ScSkR8NA44mO-gQ&branch=master)](https://app.bitrise.io/build/1d4f2322-0af4-445c-99b0-3c58723619cb)
- GitHub Actions Workflow [![Build Status](https://github.com/nevercode-rudrank/Benchmarks/actions/workflows/ios.yml/badge.svg?branch=benchmark)](https://github.com/nevercode-rudrank/Benchmarks/actions/runs/7114673613)


## [Wikipedia iOS](https://github.com/nevercode-rudrank/wikipedia-ios)

The official Wikipedia iOS app is open-sourced. It also contains multiple dependencies and hundreds of tests.

**Test name** | **Codemagic (M2 Mac Mini)** | **Codemagic (M1 Mac Mini)** | **Bitrise** | **GitHub Actions**
--- | --- | --- | --- | ---
Building Project | **1m 20s** | 1m 42s | 1m 36s | 4m 58s
Running Tests | **2m 34s** | 3m 27s | 3m 18s | 9m 3s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/codemagic.yaml)
- [`bitrise.yml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/bitrise.yml)
- [`github action ios.yml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/.github/workflows/ios.yml)

- Codemagic M2 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/6267c85aeb4a9a0e7b7eba1b/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/6267c85aeb4a9a0e7b7eba1b/build/643fa4ada6c16df739a8e5c8)
- Codemagic M1 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/6267c85aeb4a9a0e7b7eba1b/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/6267c85aeb4a9a0e7b7eba1b/build/643fa4ada6c16df739a8e5c7)
- Bitrise M1 Elite XL Workflow [![Build Status](https://app.bitrise.io/app/c8237484d99238e6/status.svg?token=N9v0ks0Fat21r-SsMluWEQ&branch=master)](https://app.bitrise.io/build/492c1e5f-51e3-4d1e-948c-eeedd323da3b)
- GitHub Actions Workflow [![Build Status](https://github.com/nevercode-rudrank/wikipedia-ios/actions/workflows/ios.yml/badge.svg)](https://github.com/nevercode-rudrank/wikipedia-ios/actions/runs/3393761012)

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

- Codemagic M2 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/63a21b433246c3f84a9da7d4/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/63a21b433246c3f84a9da7d4/build/643faf0fc112ac5cd5e19fb8)
- Codemagic M1 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps/63a21b433246c3f84a9da7d4/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/63a21b433246c3f84a9da7d4/build/643faf0fc112ac5cd5e19fb6)
