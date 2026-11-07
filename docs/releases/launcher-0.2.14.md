# TLauncher Compatible

Horizon Free launcher 0.2.14 can prepare Horizon using an existing TLauncher
Minecraft installation. It discovers the standard Windows game folder
(`%APPDATA%\.minecraft`) and can reuse a profile such as `Fabric 26.3` when its
client jar matches the Minecraft version pinned by the selected Horizon build.

Run the matching version once in TLauncher. In Horizon, open **Settings →
Minecraft folder** if you use a custom installation path, then install and
prepare a Horizon game version.

The launcher verifies the client jar and version metadata before using them.
Horizon launches as its own application and uses the fork's offline play.

The source discovery tests, including the TLauncher profile test, passed on
Linux. See the [Windows setup and build instructions](https://github.com/parthdongre/horizon-free-all-platforms#use-tlauncher-on-windows)
for the x64 build command.
