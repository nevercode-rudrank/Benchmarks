# Benchmarks

Codemagic released the powerful M1 Mac mini for the developers to build and test their apps faster. This document contains tests run on popular open-source native iOS projects to give you an idea about the fast speed in a real-world scenario and the comparison with Bitrise and GitHub Actions.

> The build times are subjective and depend on external factors like the network speed for fetching resources, project size, external third-party dependencies, number of tests, etc.

## [Xcode Benchmark](https://github.com/nevercode-rudrank/Benchmarks/tree/benchmark)

The first project is the famous `XcodeBenchmark` used to provide an idea about the performance of M1 Mac mini and Mac Pro. It is a framework that includes **42 popular CocoaPods** libraries and **70+ dependencies** in total.

**Test name** | **Codemagic** | **Bitrise** | **GitHub Actions**
--- | --- | --- | ---
Running Benchmark Tests | **184s** | 134s | 1080s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/Benchmarks/blob/benchmark/codemagic.yaml)
- [`bitrise.yml`](https://github.com/nevercode-rudrank/Benchmarks/blob/benchmark/bitrise.yml)
- [`github action ios.yml`](https://github.com/nevercode-rudrank/Benchmarks/blob/master/.github/workflows/ios.yml)

- Codemagic M1 Mac mini Workflow  [![Codemagic build status](https://api.codemagic.io/apps//636384f636dd120e8bce1532/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/636384f636dd120e8bce1532/build/6364f680030e6b1c91779158) 
- Bitrise M1 Elite XL Workflow [![Build Status](https://app.bitrise.io/app/7e4ee99efa9d94cf/status.svg?token=j-0HsuqsKi3Lx9hDmaQTag&branch=master)](https://app.bitrise.io/app/7e4ee99efa9d94cf)
- GitHub Actions Workflow ![Build Status](https://github.com/nevercode-rudrank/Benchmarks/actions/workflows/ios.yml/badge.svg?branch=benchmark)


## [Wikipedia iOS](https://github.com/nevercode-rudrank/wikipedia-ios)

The official Wikipedia iOS app is open-sourced. It also contains multiple dependencies and hundreds of tests.

**Test name** | **Codemagic** | **Bitrise** | **GitHub Actions**
--- | --- | --- | ---
Building Project | **115s** | 96s | 299s
Running Tests | **219** | 204s | 561s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/codemagic.yaml)
- [`bitrise.yml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/bitrise.yml)
- [`github action ios.yml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/.github/workflows/ios.yml)

- Codemagic M1 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps//6267c85aeb4a9a0e7b7eba1b/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/6267c85aeb4a9a0e7b7eba1b/build/6365081abf9296703e06875d)
- Bitrise M1 Elite XL Workflow [![Build Status](https://app.bitrise.io/app/c8237484d99238e6/status.svg?token=N9v0ks0Fat21r-SsMluWEQ&branch=master)](https://app.bitrise.io/app/c8237484d99238e6)
- GitHub Actions Workflow ![Build Status](https://github.com/nevercode-rudrank/wikipedia-ios/actions/workflows/ios.yml/badge.svg)
