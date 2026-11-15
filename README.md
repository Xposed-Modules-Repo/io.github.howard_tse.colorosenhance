# ColorOS 增强

作者：[Howard / Howard-Tse](https://github.com/Howard-Tse)。非 OPPO 或 OnePlus 官方产品。

[源码与反馈](https://github.com/Howard-Tse/ColorOS-Enhance) · [下载](https://github.com/Howard-Tse/ColorOS-Enhance/releases) · [旧包迁移说明](https://github.com/Howard-Tse/ColorOS-Enhance/blob/main/docs/MIGRATION.md)

## 要求

- ColorOS 16 / Android 16 或 ColorOS 17 / Android 17，最低 API 36。
- root 与支持现代 libxposed API 102 的 LSPosed 实现。
- 按功能勾选系统界面、设置、电话、系统框架、多彩引擎等作用域。首次启用或更新系统框架中的功能需要完整重启。

## 功能

- 流体云与状态栏解绑，按场景保持显示／动画补全，横竖屏配置。
- 摄像头区域展开、卡片圆角、胶囊尺寸、卡片排序和背景压暗。
- 媒体胶囊保留、可配置六频段实时律动；采集不可用时回退原厂动画。
- 状态栏图标显示规则、仅下拉显示、锁屏规则、左右跨区拖动排序。
- 状态栏电池增强、全景息屏增强、SIM PIN 自动解锁及安装器替换。
- 独立设置应用与系统设置内嵌入口，各功能组独立开关。

## 从旧包升级

新包 `io.github.howard_tse.colorosenhance` 不覆盖旧包 `dev.howard.colorosenhance`。保留旧包和数据，安装并打开新版，为新版允许 root 读取；设置会自动复制。按提示停用旧模块、启用新版及作用域，返回完成交接后完整重启。确认正常后再卸载旧包。

不导出 PIN、完整 ICCID 或密钥。检测到旧暂存 PIN 时，新版 SIM 增强暂时关闭，需要重新保存并核对卡槽。已确认的电话端凭据与每次开机尝试保护继续保留。

## 验证限制

1.30.0 为首次公开正式版本。迁移、重启、两处设置页、媒体卡片及日常手势已验收，少见自动首弹场景和桌面图标深浅刷新仍待更多验证。机型、固件和主题可能影响效果，不能保证所有 ColorOS 设备均适用。

项目原创代码采用 MIT，依赖保留各自许可。反馈不要附 PIN、账号、序列号、原始配置或完整设备日志。
