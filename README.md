# Binaries for Ungoogled Chromium on 64-bit Windows.

The best thing you could do is build it yourself, following the build process (don't forget the pypiwin32 module for Python 2.7) at:<br>
https://github.com/ungoogled-software/ungoogled-chromium-windows<br>
Remember to read the chromium install instructions and and activate "Debugging Tools For Windows":<br>
https://chromium.googlesource.com/chromium/src/+/refs/tags/81.0.4044.113/docs/windows_build_instructions.md#visual-studio<br>
Keep in mind that you can update the ungoogled-chromium submodule, should there be any newer releases not yet added to the windows repo.

Build it from cmd when running as an admin. If the build fails then try updating 7-zip, originally my older installation of 7-zip failed. Another thing to keep in mind is that because of relative paths in Windows, you should build everything in the same drive (C:\ for example) as you have Python2 and Python3 installed.

If you don't want to go through that (the compilation itself can take ~11h), this is what this repo is for.

Note also that you cannot access extensions from the Chrome Webstore with UG, you have to get the crx files directly to install extensions. The easiest way to get them would be at https://crxextractor.com/, which links directly to the crx files on Google's servers. UG also has a [wiki page about extensions](https://ungoogled-software.github.io/ungoogled-chromium-wiki/faq#can-i-install-extensions-or-themes-from-the-chrome-webstore) and how to get them.

I have provided the most recent stable versions of [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm "uBlock Origin") avaliable from the Chrome webstore, although newer releases might exist on the uBlock Origin github.

## Latest Releases

#### Ungoogled Chromium 84.0.4147.125-1 [(commit 4f57400)][84.0.4147.125-1]
[84.0.4147.125-1]: https://github.com/Eloston/ungoogled-chromium/commit/4f574006aca69964995acfa0718e7097ce36c059 "4f574006aca69964995acfa0718e7097ce36c059"
Installer and zip file both compiled and uploaded 2020-08-14 with LLVM-11.0.0-rc1 and VS19 v16.7.1.<br>
.exe installer: (link)
```
MD5:    099a89023df46c7c1d5bdc484e1ee1cd
SHA1:   099a89023df46c7c1d5bdc484e1ee1cd
SHA256: 099a89023df46c7c1d5bdc484e1ee1cd
```
.zip file: (link)
```
MD5:    099a89023df46c7c1d5bdc484e1ee1cd
SHA1:   099a89023df46c7c1d5bdc484e1ee1cd
SHA256: 099a89023df46c7c1d5bdc484e1ee1cd
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