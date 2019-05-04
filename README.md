# MaterialFox
*一个使用 userChrome.css 的MD风格的 Firefox 主题*

![Preview](https://user-images.githubusercontent.com/5405629/45172944-21d91900-b24a-11e8-8bc5-03814121b0de.png)
这个主题被糖果咖啡所充能. 如果你喜欢, 请考虑捐助我们以进行后续的开发.

[![Buy me a coffee](https://svgshare.com/i/8Yd.svg)](https://www.buymeacoffee.com/n4ho5QX2l)

## What this does
受谷歌MD风格的设计和最新的 Chrome UI 的影响, 这个主题将使你的火狐变形一个MD风格的浏览器. 目标是最可能的接近最新构建的 Google Chrome dev.

这个使用了 userChrome.css 主题, 意味着你可以手动添加到firefox项目中. The theme overrides certain browser styles. Currently, only the main UI is affected (settings pages, etc. are not). More elements of the UI may be styled in the future.

## Installation
Some steps involve accessing the about:config page. You can get there by typing it into your urlbar.

### Mandatory instructions
1. Copy the chrome folder into your Firefox profile directory. To find your profile directory, go to about:support. Alternatively, you can symlink your chrome folder instead of copying.
2. [about:config] Set ```svg.context-properties.content.enabled``` to ```true``` (default is ```false```).
3. Restart Firefox.

### Recommended instructions
Add space above tab bar:
* Right click on toolbar -> Customize.
* Check Drag Space checkbox.

Emulate Chrome's profile switcher button:
* Right click on toolbar -> Customize.
* Drag Synced Tabs to the toolbar.

Replicate Chrome behaviour for clipped tabs:
* [about:config] Set ```browser.tabs.tabClipWidth``` to ```83``` (default is ```144```).

Allow tabs to shrink more; tabs in overflow will look the same as pinned tabs:
* [about:config] Add new entry ```materialFox.reduceTabOverflow``` with value ```true```.

Replicate Chrome's "Not Secure" on HTTP:
* [about:config] Set ```security.insecure_connection_text.enabled``` to ```true```.

## Please note
* Linux is not frequently tested; last tested on 07/09/2018.
* Some customisation settings may no longer work (such as compact density).
* Some custom themes may clash with address bar.
