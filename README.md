# Flipper for Apple Slicon

Flipper macOS application currents runs via Rosetta on Apple Silicon machines and therefore suffers from performance issues. fps is super low and there is a noticable lag while switching between plugins, etc.

Performance is great on the generated Flipper universal binary, didn't see any frame drops at all, runs super smooth. (Can be downloaded from the [releases](https://github.com/chiragramani/FlipperReleases/releases) section)

This is being tracked in https://github.com/facebook/flipper/pull/3553. Until Meta distributes a universal Flipper binary, this repository applies the author's commits on every latest Flipper release via a GitHub Action workflows. The `generate.sh` is the file executed by the workflow.

Additional patch applied:
1. Using https://www.npmjs.com/package/@electron/universal 2.0.0 as this is the latest stable release. 


Note: this repository will be deleted when Meta starts distributing a universal Flipper binary.
