# Contributing to LibPdIntegration

Thanks for considering contributing to LibPdIntegration!

At the time of writing, what the project needs most urgently is people who are willing and able to build libpd binaries for non-Windows platforms. The current binaries are all built to different versions of libpd, some of which contain notable bugs which have since been fixed on the [libpd master branch](https://github.com/libpd/libpd). What's worse is there's no documentation of which versions the binaries we do have were built to 😱

If you're willing to build binaries for any of the following platforms, please get in touch via [issue #20](https://github.com/LibPdIntegration/LibPdIntegration/issues/20) so we can coordinate versions and start to get the binaries better organised. We need binaries for:

- Mac OSX (see also [issue #21](https://github.com/LibPdIntegration/LibPdIntegration/issues/21))
- Linux
- iOS
- Android

There are [generic instructions for building libpd binaries on the wiki](https://github.com/LibPdIntegration/LibPdIntegration/wiki/building-your-own-libpd-binaries), in addition to [specific instructions for building an iOS binary](https://github.com/LibPdIntegration/LibPdIntegration/wiki/iOS). Please do ensure you build any binaries with the MULTI and UTIL flags, as otherwise the binaries will not work with LibPdIntegration.

## Reporting Issues

Beyond that, if you've spotted a bug or have a feature request, first [check if there's an existing issue about it](https://github.com/LibPdIntegration/LibPdIntegration/issues), and if not, [post a new issue](https://github.com/LibPdIntegration/LibPdIntegration/issues).

## Submitting Pull Requests

If you're interested in contributing code, please keep pull requests focused on a single task/topic. If you're new to Pull Requests, the general procedure (assuming command-line git) is:

1. Fork the LibPdIntegration repo on github.
2. Clone your fork: `git clone https://github.com/<your-username>/<project-name>`
3. Navigate to your newly cloned directory: `cd project-name`
4. Create a new branch for the feature: `git checkout -b my-new-feature`
5. Make your changes.
6. Commit your changes: `git commit -am "Explanation of changes."`
7. Push to your branch: `git push origin my-new-feature`
8. [Submit a pull request](https://github.com/LibPdIntegration/LibPdIntegration/pulls) with a full explanation of your changes.