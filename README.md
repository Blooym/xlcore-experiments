# XIVLauncher.Core Experimental Builds
This repository hosts experimental and beta versions of XIVLauncher.Core for testing.

> [!WARNING]  
> These builds are not supported outside of our dedicated testing feedback spaces. Please do not report issues with these builds anywhere else, including the primary XIVLauncher.Core repository.
>
> **Additionally, while they are usually tested by a developer beforehand, these builds are not guarenteed to be stable. Only use them if you are comfortable resolving things manually and make regular backups of your data beforehand.**

## How to use experimental builds

### Prerequisites
The only recommended way to use experimental builds is with [XLM](https://github.com/Blooym/XLM), which handles automatic updates. Other methods are not provided here at this time.

### Installation steps
1. Find the build name via the [Current Experimental Builds](#current-experimental-builds) section below
2. Add the following to your Steam Launch Arguments, replacing `BUILD_NAME` with your chosen build:
   ```
   --xlcore-web-release-url="https://github.com/Blooym/xlcore-experiments/releases/download/BUILD_NAME/"
   ```
3. Restart the launcher

### Important notes
- You cannot use experimental builds if you have `--xlcore-repo-owner`, `--xlcore-repo-name`, or `--xlcore-release-asset` in your launch options. Remove these first.
  
- To switch back to stable releases, simply remove the experimental build argument from your launch options and restart.

- When an experimental build is removed from this repository, it becomes unavailable. You must remove the launch argument to return to stable releases, or else the you will not receive essential updates and the launcher may fail to start.

## Current experimental builds
| Build Name | Description | Source |
|------------|-------------|--------|
| `experiment-newimgui` | New ImGui backend implementation | [PR #281](https://github.com/goatcorp/XIVLauncher.Core/pull/281) |
