# hello-world

`com.calvinx.hello-world` is a third-party HelloHQ plugin. It is the same
shape as HelloHQ's official hello-world: a Tier-2 Wasm component that reads
portfolio names and returns a declarative list.

The id prefix `com.calvinx.` is this publisher's namespace. The plugin is
meant to be installed as Verified, under an author certificate for
[calvinchengx](https://github.com/calvinchengx), not under HelloHQ's Official
keys.

## Build

Requires the `wasm32-unknown-unknown` target and `wasm-tools` 1.252 or newer.

```sh
./build.sh
```

`build.sh` prints the SHA-256 of `plugin.wasm`. That hash belongs in
`manifest.json` when a `v1.0.0` release is cut. The hash in the manifest is
still the placeholder, and no release has been published.

The Rust SDK is vendored from HelloHQ/plugin-sdk `sdks/rust` at `c567a89`
until that crate is on crates.io.
