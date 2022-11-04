# Benchmarks

Codemagic released the powerful M1 Mac mini for the developers to build and test their apps faster. This document contains tests run on popular open-source native iOS projects to give you an idea about the fast speed in a real-world scenario and the comparison with Bitrise and GitHub Actions.

> The build times are subjective and depend on external factors like the network speed for fetching resources, project size, external third-party dependencies, number of tests, etc.

## [Xcode Benchmark](https://github.com/devMEremenko/XcodeBenchmark)

The first project is the famous `XcodeBenchmark` used to provide an idea about the performance of M1 Mac mini and Mac Pro. It is a framework that includes **42 popular CocoaPods** libraries and **70+ dependencies** in total.

**Test name** | **Codemagic** | **Bitrise** | **GitHub Actions**
--- | --- | --- | ---
Running Benchmark Tests | **184s** | 134s | 1600s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/XcodeBenchmark/blob/master/codemagic.yaml)

- M1 Mac mini Workflow [![Codemagic build status](https://api.codemagic.io/apps//636384f636dd120e8bce1532/ios-m1-mac-mini-workflow/status_badge.svg)](https://codemagic.io/app/636384f636dd120e8bce1532/build/6364f680030e6b1c91779158)

## [Wikipedia iOS](https://github.com/wikimedia/wikipedia-ios)

The official Wikipedia iOS app is open-sourced. It also contains multiple dependencies and hundreds of tests.

**Test name** | **Codemagic** | **Bitrise** | **GitHub Actions**
--- | --- | --- | ---
Building Project | **120s** | 96s | 259s
Running Tests | **233** | 204s | 422s

- [`codemagic.yaml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/codemagic.yaml)
- [`bitrise.yml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/bitrise.yml)
- [`github action ios.yml`](https://github.com/nevercode-rudrank/wikipedia-ios/blob/main/.github/workflows/ios.yml)

