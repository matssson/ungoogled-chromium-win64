# Binaries for Ungoogled Chromium on 64-bit Windows

## Building Ungoogled Chromium

The best thing you could do is build it yourself, following the build process at:<br>
https://github.com/ungoogled-software/ungoogled-chromium-windows (don't forget pypiwin32 for Python 2.7)

Remember to read the chromium install instructions and and activate "Debugging Tools For Windows".<br>
https://chromium.googlesource.com/chromium/src/+/refs/tags/81.0.4044.113/docs/windows_build_instructions.md#visual-studio

Also keep in mind that you can update the ungoogled-chromium submodule if there are any newer releases not yet added to the windows repo.

Build it from cmd when running as an admin. If the build fails then try updating 7-zip, originally my older installation of 7-zip failed. Another thing to keep in mind is that because of relative paths in Windows, you should build everything in the same drive (C:\ for example) as you have Python2 and Python3 installed. The compilation itself can take ~10h.

Note that you cannot access extensions from the Chrome Webstore with UG, you have to get the crx files directly to install extensions. The easiest way to get them would be at https://crxextractor.com/, which links directly to the crx files on Google's servers. UG also has a [wiki page about extensions](https://ungoogled-software.github.io/ungoogled-chromium-wiki/faq#can-i-install-extensions-or-themes-from-the-chrome-webstore) and how to get them.

This repo is for providing prebuilt win64 binaries in the form of executable installers and embeddable zip files. I have also provided the most recent stable versions of [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm "uBlock Origin") that are avaliable on the Chrome webstore, although newer releases might exist on the uBlock Origin github.

## Latest Releases

#### Ungoogled Chromium 84.0.4147.125-1 [(commit 4f57400)][84.0.4147.125-1]
[84.0.4147.125-1]: https://github.com/Eloston/ungoogled-chromium/commit/4f574006aca69964995acfa0718e7097ce36c059 "4f574006aca69964995acfa0718e7097ce36c059"
Installer and zip file both compiled and uploaded 2020-08-14 with LLVM-11.0.0-rc1 and VS19 v16.7.1.<br>
.exe installer: [ungoogled-chromium_84.0.4147.125-1.1_installer.exe](ug-installer/ungoogled-chromium_84.0.4147.125-1.1_installer.exe)
```
MD5:    9711D0DA192A65BA986E6F677D4E2AC3
SHA1:   AC00FCB830713822B102D92CD59AE1E1004B7142
SHA256: D323D9FC48FC08250361A3C0EA35931404F94BC78FD503597EAC5A282DEA5D97
```
.zip file: [ungoogled-chromium_84.0.4147.125-1.1_windows.zip](ug-zip/ungoogled-chromium_84.0.4147.125-1.1_windows.zip)
```
MD5:    92D060321A7E2016A9D9C11863E89CBF
SHA1:   7CABB128C7B85E60201BC40E15EB20F522A76AA4
SHA256: E0F18A396051AF81FC61EF390FA789C171EA6641C3F8CC4696FE9ADA52D9E703
```

#### uBlock Origin 1.28.4
Updated at 2020-07-25, mirrored 2020-08-13 from Chrome webstore, via the [following link.](https://clients2.googleusercontent.com/crx/blobs/QwAAAHF3InbmK-wFIemaY3I3BCPrqnoL_LJfgHaCGizREm5Fe6K-3m6WlgeLY8I8vyxgijJqqbP95OEXLN_02II6a5j1ia4dH4VkHftHTxr9d9GQAMZSmuXtXtwquCecAwgmgDNHBp4ql3OLgA/extension_1_28_4_0.crx)<br>
.crx file: [extension_1_28_4_0.crx](ublock/extension_1_28_4_0.crx)
```
MD5:    AD5DE970776C3C6AA65B0B4794BF726C
SHA1:   E7CC10FE3DB4E6A1CE1E5D54E4BF4CEE8AD8574D
SHA256: 0D324C1E1C1EB1F6BFC9BE69794DA3015CB15B218D5A9508A6BA4D2C26E48957
```

## Older Releases
In future