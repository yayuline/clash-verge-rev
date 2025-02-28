## v1.5.8

### Features

- 优化 UI 细节
- Linux 绘制窗口圆角
- 开放 DevTools

### Bugs Fixes

- 修复 MacOS 下开启 Tun 内核崩溃的问题

---

## v1.5.7

### Features

- 优化 UI 各种细节
- 提供菜单栏图标样式切换选项(单色/彩色/禁用)
- 添加自动检查更新开关
- MacOS 开启 Tun 模式自动修改 DNS
- 调整可拖动区域(尝试修复触摸屏无法拖动的问题)

---

## v1.5.6

### Features

- 全新专属 Verge rev UI 界面 (by @Amnesiash) 及细节调整
- 提供允许无效证书的开关
- 删除不必要的快捷键
- Provider 更新添加动画
- Merge 支持 Provider
- 更换订阅框的粘贴按钮，删除默认的"Remote File" Profile 名称
- 链接菜单添加节点显示

### Bugs Fixes

- Linux 下图片显示错误

---

## v1.5.4

### Features

- 支持自定义托盘图标
- 支持禁用代理组图标
- 代理组显示当前代理
- 修改 `打开面板` 快捷键为`打开/关闭面板`

---

## v1.5.3

### Features

- Tun 设置添加重置按钮

### Bugs Fixes

- Tun 设置项显示错误的问题
- 修改一些默认值
- 启动时不更改启动项设置

---

## v1.5.2

### Features

- 支持自定义延迟测试超时时间
- 优化 Tun 相关设置

### Bugs Fixes

- Merge 操作出错
- 安装后重启服务
- 修复管理员权限启动时开机启动失效的问题

---

## v1.5.1

### Features

- 保存窗口最大化状态
- Proxy Provider 显示数量
- 不再提供 32 位安装包（因为 32 位经常出现各种奇怪问题，比如 tun 模式无法开启；现在系统也几乎没有 32 位了）

### Bugs Fixes

- 优化设置项名称
- 自定义 GLOBAL 代理组时代理组显示错误的问题

---

## v1.5.0

### Features

- 删除 Clash 字段过滤功能
- 添加 socks 端口和 http 端口设置
- 升级内核到 1.18.1

### Bugs Fixes

- 修复 32 位版本无法显示流量信息的问题

---

## v1.4.11

### Break Changes

- 此版本更改了 Windows 安装包安装模式，需要卸载后手动安装，否则无法安装到正确位置

### Features

- 优化了系统代理开启的代码，解决了稀有场景下代理开启卡顿的问题
- 添加 MacOS 下的 debug 日志，以便日后调试稀有场景下 MacOS 下无法开启系统代理的问题
- MacOS 关闭 GUI 时同步杀除后台 GUI [#306](https://github.com/clash-verge-rev/clash-verge-rev/issues/306)

### Bugs Fixes

- 解决自动更新时文件占用问题
- 解决稀有场景下系统代理开启失败的问题
- 删除冗余内核代码

---

## v1.4.10

### Features

- 设置中添加退出按钮
- 支持自定义软件启动页
- 在 Proxy Provider 页面展示订阅信息
- 优化 Provider 支持

### Bugs Fixes

- 更改端口时立即重设系统代理
- 网站测试超时错误

---

## v1.4.9

### Features

- 支持启动时运行脚本
- 支持代理组显示图标
- 新增测试页面

### Bugs Fixes

- 连接页面时间排序错误
- 连接页面表格宽度优化

---

## v1.4.8

### Features

- 连接页面总流量显示

### Bugs Fixes

- 连接页面数据排序错误
- 新建订阅时设置更新间隔无效
- Windows 拨号网络无法设置系统代理
- Windows 开启/关闭系统代理延迟(使用注册表即可)
- 删除无效的背景模糊选项

---

## v1.4.7

### Features

- Windows 便携版禁用应用内更新
- 支持代理组 Hidden 选项
- 支持 URL Scheme(MacOS & Linux)

---

## v1.4.6

### Features

- 更新 Clash Meta(mihomo) 内核到 v1.18.0
- 支持 URL Scheme(暂时仅支持 Windows)
- 添加窗口置顶按钮
- UI 优化调整

### Bugs Fixes

- 修复一些编译错误
- 获取订阅名称错误
- 订阅信息解析错误

---

## v1.4.5

### Features

- 更新 MacOS 托盘图标样式(@gxx2778 贡献)

### Bugs Fixes

- Windows 下更新时无法覆盖`clash-verge-service.exe`的问题(需要卸载重装一次服务，下次更新生效)
- 窗口最大化按钮变化问题
- 窗口尺寸保存错误问题
- 复制环境变量类型无法切换问题
- 某些情况下闪退的问题
- 某些订阅无法导入的问题

---

## v1.4.4

### Features

- 支持 Windows aarch64(arm64) 版本
- 支持一键更新 GeoData
- 支持一键更新 Alpha 内核
- MacOS 支持在系统代理时显示不同的托盘图标
- Linux 支持在系统代理时显示不同的托盘图标
- 优化复制环境变量逻辑

### Bugs Fixes

- 修改 PID 文件的路径

### Performance

- 优化创建窗口的速度

---

## v1.4.3

### Break Changes

- 更改配置文件路径到标准目录(可以保证卸载时没有残留)
- 更改 appid 为 `io.github.clash-verge-rev.clash-verge-rev`
- 建议卸载旧版本后再安装新版本，该版本安装后不会使用旧版配置文件，你可以手动将旧版配置文件迁移到新版配置文件目录下

### Features

- 移除页面切换动画
- 更改 Tun 模式托盘图标颜色
- Portable 版本默认使用当前目录作为配置文件目录
- 禁用 Clash 字段过滤时隐藏 Clash 字段选项
- 优化拖拽时光标样式

### Bugs Fixes

- 修复 windows 下更新时没有关闭内核导致的更新失败的问题
- 修复打开文件报错的问题
- 修复 url 导入时无法获取中文配置名称的问题
- 修复 alpha 内核无法显示内存信息的问题

---

## v1.4.2

### Features

- update clash meta core to mihomo 1.17.0
- support both clash meta stable release and prerelease-alpha release
- fixed the problem of not being able to set the system proxy when there is a dial-up link on windows system [#833](https://github.com/zzzgydi/clash-verge/issues/833)
- support new clash field
- support random mixed port
- add windows x86 and linux armv7 support
- support disable tray click event
- add download progress for updater
- support drag to reorder the profile
- embed emoji fonts
- update depends
- improve UI style

---

## v1.4.1

### Features

- update clash meta core to newest 虚空终端(2023.11.23)
- delete clash core UI
- improve UI
- change Logo to original

---

## v1.4.0

### Features

- update clash meta core to newest 虚空终端
- delete clash core, no longer maintain
- merge Clash nyanpasu changes
- remove delay display different color
- use Meta Country.mmdb
- update dependencies
- small changes here and there

---

## v1.3.8

### Features

- update clash meta core
- add default valid keys
- adjust the delay display interval and color

### Bug Fixes

- fix connections page undefined exception

---

## v1.3.7

### Features

- update clash and clash meta core
- profiles page add paste button
- subscriptions url textfield use multi lines
- set min window size
- add check for updates buttons
- add open dashboard to the hotkey list

### Bug Fixes

- fix profiles page undefined exception

---

## v1.3.6

### Features

- add russian translation
- support to show connection detail
- support clash meta memory usage display
- support proxy provider update ui
- update geo data file from meta repo
- adjust setting page

### Bug Fixes

- center the window when it is out of screen
- use `sudo` when `pkexec` not found (Linux)
- reconnect websocket when window focus

### Notes

- The current version of the Linux installation package is built by Ubuntu 20.04 (Github Action).

---

## v1.3.5

### Features

- update clash core

### Bug Fixes

- fix blurry system tray icon (Windows)
- fix v1.3.4 wintun.dll not found (Windows)
- fix v1.3.4 clash core not found (macOS, Linux)

---

## v1.3.4

### Features

- update clash and clash meta core
- optimize traffic graph high CPU usage when window hidden
- use polkit to elevate permission (Linux)
- support app log level setting
- support copy environment variable
- overwrite resource file according to file modified
- save window size and position

### Bug Fixes

- remove fallback group select status
- enable context menu on editable element (Windows)

---

## v1.3.3

### Features

- update clash and clash meta core
- show tray icon variants in different system proxy status (Windows)
- close all connections when mode changed

### Bug Fixes

- encode controller secret into uri
- error boundary for each page

---

## v1.3.2

### Features

- update clash and clash meta core

### Bug Fixes

- fix import url issue
- fix profile undefined issue

---

## v1.3.1

### Features

- update clash and clash meta core

### Bug Fixes

- fix open url issue
- fix appimage path panic
- fix grant root permission in macOS
- fix linux system proxy default bypass

---

## v1.3.0

### Features

- update clash and clash meta
- support opening dir on tray
- support updating all profiles with one click
- support granting root permission to clash core(Linux, macOS)
- support enable/disable clash fields filter, feel free to experience the latest features of Clash Meta

### Bug Fixes

- deb add openssl depend(Linux)
- fix the AppImage auto launch path(Linux)
- fix get the default network service(macOS)
- remove the esc key listener in macOS, cmd+w instead(macOS)
- fix infinite retry when websocket error

---

## v1.2.3

### Features

- update clash
- adjust macOS window style
- profile supports UTF8 with BOM

### Bug Fixes

- fix selected proxy
- fix error log

---

## v1.2.2

### Features

- update clash meta
- recover clash core after panic
- use system window decorations(Linux)

### Bug Fixes

- flush system proxy settings(Windows)
- fix parse log panic
- fix ui bug

---

## v1.2.1

### Features

- update clash version
- proxy groups support multi columns
- optimize ui

### Bug Fixes

- fix ui websocket connection
- adjust delay check concurrency
- avoid setting login item repeatedly(macOS)

---

## v1.2.0

### Features

- update clash meta version
- support to change external-controller
- support to change default latency test URL
- close all connections when proxy changed or profile changed
- check the config by using the core
- increase the robustness of the program
- optimize windows service mode (need to reinstall)
- optimize ui

### Bug Fixes

- invalid hotkey cause panic
- invalid theme setting cause panic
- fix some other glitches

---

## v1.1.2

### Features

- the system tray follows i18n
- change the proxy group ui of global mode
- support to update profile with the system proxy/clash proxy
- check the remote profile more strictly

### Bug Fixes

- use app version as default user agent
- the clash not exit in service mode
- reset the system proxy when quit the app
- fix some other glitches

---

## v1.1.1

### Features

- optimize clash config feedback
- hide macOS dock icon
- use clash meta compatible version (Linux)

### Bug Fixes

- fix some other glitches

---

## v1.1.0

### Features

- add rule page
- supports proxy providers delay check
- add proxy delay check loading status
- supports hotkey/shortcut management
- supports displaying connections data in table layout(refer to yacd)

### Bug Fixes

- supports yaml merge key in clash config
- detect the network interface and set the system proxy(macOS)
- fix some other glitches

---

## v1.0.6

### Features

- update clash and clash.meta

### Bug Fixes

- only script profile display console
- automatic configuration update on demand at launch

---

## v1.0.5

### Features

- reimplement profile enhanced mode with quick-js
- optimize the runtime config generation process
- support web ui management
- support clash field management
- support viewing the runtime config
- adjust some pages style

### Bug Fixes

- fix silent start
- fix incorrectly reset system proxy on exit

---

## v1.0.4

### Features

- update clash core and clash meta version
- support switch clash mode on system tray
- theme mode support follows system

### Bug Fixes

- config load error on first use

---

## v1.0.3

### Features

- save some states such as URL test, filter, etc
- update clash core and clash-meta core
- new icon for macOS

---

## v1.0.2

### Features

- supports for switching clash core
- supports release UI processes
- supports script mode setting

### Bug Fixes

- fix service mode bug (Windows)

---

## v1.0.1

### Features

- adjust default theme settings
- reduce gpu usage of traffic graph when hidden
- supports more remote profile response header setting
- check remote profile data format when imported

### Bug Fixes

- service mode install and start issue (Windows)
- fix launch panic (Some Windows)

---

## v1.0.0

### Features

- update clash core
- optimize traffic graph animation
- supports interval update profiles
- supports service mode (Windows)

### Bug Fixes

- reset system proxy when exit from dock (macOS)
- adjust clash dns config process strategy

---

## v0.0.29

### Features

- sort proxy node
- custom proxy test url
- logs page filter
- connections page filter
- default user agent for subscription
- system tray add tun mode toggle
- enable to change the config dir (Windows only)

---

## v0.0.28

### Features

- enable to use clash config fields (UI)

### Bug Fixes

- remove the character
- fix some icon color

---

## v0.0.27

### Features

- supports custom theme color
- tun mode setting control the final config

### Bug Fixes

- fix transition flickers (macOS)
- reduce proxy page render

---

## v0.0.26

### Features

- silent start
- profile editor
- profile enhance mode supports more fields
- optimize profile enhance mode strategy

### Bug Fixes

- fix csp restriction on macOS
- window controllers on Linux

---

## v0.0.25

### Features

- update clash core version

### Bug Fixes

- app updater error
- display window controllers on Linux

### Notes

If you can't update the app properly, please consider downloading the latest version from github release.

---

## v0.0.24

### Features

- Connections page
- add wintun.dll (Windows)
- supports create local profile with selected file (Windows)
- system tray enable set system proxy

### Bug Fixes

- open dir error
- auto launch path (Windows)
- fix some clash config error
- reduce the impact of the enhanced mode

---

## v0.0.23

### Features

- i18n supports
- Remote profile User Agent supports

### Bug Fixes

- clash config file case ignore
- clash `external-controller` only port
