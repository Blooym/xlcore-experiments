# xlcore-experiments
This repository is for releases of experimental/beta builds of XIVLauncher.Core that are used for semi-public testing.

> [!WARNING]  
> These builds are not supported outside of our dedicated testing feedback spaces. Please do not report issues with these builds anywhere else, including the primary XIVLauncher.Core repository.
>
> **Additionally, while they are usually tested by a developer beforehand, these builds are not guarenteed to be stable. Only use them if you are comfortable resolving things manually and make regular backups of your data beforehand.**

## Using experimental builds

Currently the only recommended way to opt into a experimental build is by using [XLM](https://github.com/Blooym/XLM) as it provides an easy method for automatic updates. Follow the instructions below to opt in to a build, replacing the `BUILD_NAME` placeholder with the name of the build you'd like to use.

In your Steam Launch Arguments, add the following:
```
--xlcore-web-release-url="https://github.com/Blooym/xlcore-experiments/releases/download/BUILD_NAME/"
```
  - *You cannot opt in to beta builds of XIVLauncher.Core while you have `--xlcore-repo-owner`, `--xlcore-repo-name` or `--xlcore-release-asset` configured in your launch options. Please remove them if you wish to use an experimental build.*
  - *If at any time you wish to switch back to stable release builds, simply remove the given launch argument and restart the launcher.*

After an experimental build has been removed, the build will become unavailable for download. You will need to remove the experiment launch argument above to move back to the stable release again, otherwise you will not receive essential updates and may not be able to launch at all until you do.
