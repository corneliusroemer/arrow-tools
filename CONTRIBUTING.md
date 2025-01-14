# Contribution guide

Thank you for investing your time in contributing to this project! We appreciate all kinds of contributions ranging from filing issues,comments on issues, pull requests, and code reviews.

## Issues

When creating an issue, search for existing issues. Provide a minimal, reproducible example and explain your configuration. Please keep in mind that the maintainers of this project are volunteers and may not have the time to debug your issue.

## Pull requests

We welcome pull requests. If a pull request fixes an existing issue, include `fixes #XXX` in the description. For the pull request title, please use the [conventional commit](https://www.conventionalcommits.org/en/v1.0.0/) format (e.g. `fix: do not crash on empty input`). If you make a contribution in one repo, after a review, please migrate the fix (if applicable) to the other repos ([csv2parquet](https://github.com/domoritz/csv2parquet), [json2parquet](https://github.com/domoritz/json2parquet), [csv2arrow](https://github.com/domoritz/csv2arrow), or [json2arrow](https://github.com/domoritz/json2arrow)).

Please make sure that your code is formatted correctly and passes some automated tests. To format and check the code, run

```bash
cargo clippy && cargo fmt
```

## Making a release

We use [`cargo-release`](https://github.com/crate-ci/cargo-release/tree/master) to make releases, which you can install with `cargo binstall cargo-release` or `cargo install cargo-release`.

The run `cargo release LEVEL` such as `cargo release minor` as a dry run. When everything works, add `--execute`.
