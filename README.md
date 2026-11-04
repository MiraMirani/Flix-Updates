# Flix updates

Public installers and app configuration. The app source stays in the private Flix repository.

## Change the website

Edit **config.json** on GitHub, change `primaryDomain`, then commit. Add compatible HTTPS mirror addresses to `fallbackDomains` if needed. Do not include movie paths, passwords or tokens.

Apps in Automatic domain mode read this file before loading the catalog. They try the listed domains, then the last working address and built-in default. If GitHub is unavailable they use cached configuration. Manual website settings are preserved. Domain changes apply at the next launch, not during playback. GitHub caching may delay changes by a few minutes.

## Downloads

Open [Releases](https://github.com/MiraMirani/Flix-Updates/releases). Tags begin with `android-tv-`, `macos-` or `windows-`. Each platform has its own version.

Apps check for updates at launch and through **Check for updates**. Downloading is optional; installation requires your confirmation. Older builds need one manual update to gain these features.

The `releases` section is maintained by the publishing tool. Edit the domain fields only. Never put private source archives in this repository.
