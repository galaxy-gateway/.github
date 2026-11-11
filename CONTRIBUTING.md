# Contributing to Galaxy Gateway

Thanks for helping. This guide applies to every repository in the org unless that repo has its own CONTRIBUTING.md.

## Where to start

Find the project in the [hub catalog](https://github.com/galaxy-gateway/galaxy-gateway). Repos marked `active` welcome pull requests. Repos marked `experiment` or `cold` welcome issues first, so we can agree on direction before you write code.

## Issues first

For anything bigger than a small fix, open an issue before the pull request. Larger changes get a short plan in the repo's `docs/plans/` directory.

## Setup

Clone the single repo you want to change. To work on the whole org at once, install the `meta` CLI (`cargo install metarepo`), clone the hub, and run `meta git clone`. See the hub docs for details.

## Commits

- Use conventional commits, for example `fix(parser): handle empty input`.
- Keep subjects plain ASCII.
- Put one `Closes #N` per line in the body, one line for each issue.
- Sign off every commit (DCO): `git commit -s`. This adds a `Signed-off-by` line certifying you have the right to submit the change under the repo license (https://developercertificate.org).
- Maintainers sign commits with GPG or SSH. It is encouraged for everyone.

## Definition of done

- Rust: `cargo build`, `cargo test`, `cargo clippy -- -D warnings`, and `cargo fmt --check` all pass.
- Deno: `deno task check` passes.
- Other repos: run whatever the repo README names.

## AI-assisted contributions

Welcome. The human submitting the change is responsible for it, must have run it, and signs the DCO for it.

## Review

One maintainer approval and green CI. We squash merge.

## Security issues

Never in public issues. See [SECURITY.md](SECURITY.md).

## License

Your contribution is licensed under the license of the repository you contribute to.

## Code of Conduct

We follow the [Contributor Covenant 2.1](CODE_OF_CONDUCT.md).
