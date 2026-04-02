这是一款通过AppleScript编写的自动化脚本，可通过此脚本自动**开启 Sidecar** 连接你的ipad，替代手动**开启 Sidecar** 。

### ⚠️ **开启 Sidecar** 前提条件：

- iPad 与 Mac 两台设备都登录了**同一个 Apple ID**
- iPad 与 Mac 连接到同一个 Wi-Fi 网络。
- [请确保您的 iPad 与 Mac 支持随航功能](https://support.apple.com/zh-cn/102597)。
- 辅助功能开启自动化脚本权限。

### 📖 功能说明

- 支持 macOS 26 (Tahoe) ，并向下兼容
- 突破性的定位方式：URL Scheme
- 智能递归查找
- 模糊匹配与属性读取
- 健壮的音量与状态管理
- 错误反馈

### 🏹 执行流程

1.  直接打开显示器设置页
2.  等待窗口加载
3. 递归寻找
4. 寻找并点击目标设备

### 🔧 工具函数

| 名称 | 功能 |
| --- | --- |
| on playSound(path) | 播放系统提供的音效 |
| on waitForApp(appName, maxSeconds) |  等待窗口加载 |
| on findAddButton(theElement,currentDepth) | 递归查找具有菜单功能的按钮 (适配不同系统版本) |
| on selectDeviceFromMenu(btn) | 从菜单中识别并点击设备 |

### 递归列出所有按钮信息
在脚本编辑器运行：ButtonPrint.scpt
