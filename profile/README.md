# Nextest

Welcome to the GitHub organization for **cargo-nextest**, a next-generation test runner for Rust. Nextest is [up to 3x](https://nexte.st/book/benchmarks) as fast as `cargo test`, and has [many features](https://nexte.st/#features) to address real-world problems with running Rust tests at scale.

Nextest is flexible to meet your needs: you can use as many or as few of its features as you like. It is used by organizations of all sizes, from individual developers to the largest corporations.

For more information, see [the nextest site](https://nexte.st/).

## Repositories in this organization

This organization contains several repositories. The ones most likely of interest to external consumers are:

* [**nextest-rs/nextest**](https://github.com/nextest-rs/nextest): The main nextest repository.

* [**nextest-rs/datatest-stable**](https://github.com/nextest-rs/datatest-stable): A library that takes a set of files on disk and turns each of them into a separate test 
case.

  This library works with nextest, and also serves as an example for how to write [custom test harnesses](https://nexte.st/book/custom-test-harnesses.html).

* [**nextest-rs/future-queue**](https://github.com/nextest-rs/future-queue): A library that permits futures to be run with a specific amount of overall concurrency. This is a generalization of [`StreamExt::buffer_unordered`](https://docs.rs/futures/latest/futures/stream/trait.StreamExt.html#method.buffer_unordered), with several additional features.

  This library is used to implement two of nextest's features: assigning [some tests a different weight](https://nexte.st/book/threads-required), and creating [groups of tests](https://nexte.st/book/test-groups) with more limited concurrency.
  
## People

The primary maintainer of nextest is [Rain (@sunshowers)](https://github.com/sponsors/sunshowers). If nextest has been useful to you or your organization, please consider [a sponsorship](https://github.com/sponsors/sunshowers).
