<h1 align="center">Jellyfin AniDB Plugin</h1>
<h3 align="center">Part of the <a href="https://jellyfin.media">Jellyfin Project</a></h3>

<p align="center">
<img alt="Plugin Banner" src="https://raw.githubusercontent.com/jellyfin/jellyfin-ux/master/plugins/SVG/jellyfin-plugin-anidb.svg?sanitize=true"/>
<br/>
<br/>
<a href="https://github.com/jellyfin/jellyfin-plugin-anidb/actions?query=workflow%3A%22Test+Build+Plugin%22">
<img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/jellyfin/jellyfin-plugin-anidb/Test%20Build%20Plugin.svg">
</a>
<a href="https://github.com/jellyfin/jellyfin-plugin-anidb/blob/master/LICENSE">
<img alt="GPLv2 License" src="https://img.shields.io/github/license/jellyfin/jellyfin-plugin-anidb.svg"/>
</a>
<a href="https://github.com/jellyfin/jellyfin-plugin-anidb/releases">
<img alt="Current Release" src="https://img.shields.io/github/release/jellyfin/jellyfin-plugin-anidb.svg"/>
</a>
</p>


## About

This plugin adds the metadata provider for [aniDB](https://anidb.net/).


## Installation

~~[See the official documentation for install instructions](https://jellyfin.org/docs/general/server/plugins/index.html#installing).~~

In Jellyfin v10.6.0 or newer version, you can install this plugin by adding repository directly.

Repository URL: https://raw.githubusercontent.com/john123951/jellyfin-plugin-anidb-cn/master/manifest.json

For version older than v10.6.0, please try the way below:

Download from release page or compile by yourself.
Decompress the package, and put the "AniDB-Cn" directory as the subdirectory of "plugins" in Jellyfin.
For Linux, it's in "~/.local/jellyfin/config/plugins"
For Mac, it's in "~/.local/share/jellyfin/plugins"
For Docker, it's in "/config/plugins" inner Docker
For Windows 10, it's in "C:\ProgramData\Jellyfin\Server\plugins" if using Administrator.
For other system, if you cannot find it, please let me know.
Restart the Jellyfin service.


## Build

1. To build this plugin you will need [.Net 6.x](https://dotnet.microsoft.com/download/dotnet/6.0).

2. Build plugin with following command
  ```
  dotnet publish --configuration Release --output bin
  ```

3. Place the dll-file in the `plugins/anidb` folder (you might need to create the folders) of your JF install


## Licence

This plugins code and packages are distributed under the GPLv2 License. See [LICENSE](./LICENSE) for more information.
