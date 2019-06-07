# MIUI Google Play DF-DFERH-01 fix

Fix Google Play DF-DFERH-01 issues on MIUI Chinese version.

修复国行 MIUI 打开 Google Play 始终提示 DF-DFERH-01 的问题

## Problem descripion / 问题描述

**<!> IMPORTANT NOTE:** Only Chinese version MIUI has this problem. NEVER install this module if you're NOT Chinese version user.

自带 Google 服务框架的国行 MIUI，**即使设置全局代理**，打开 Google Play 仍然提示 DF-DFERH-01.

反复对 Play Store/Service 清除数据、插拔 SIM 卡均无效。在其他第三方 ROM 上 Play 正常使用。

使用 adb logcat 查看日志，到关于请求的 404 错误。

## How it works / 模块工作原理

Invalidate `/system/etc/permissions/services.cn.google.xml`

无效化 `/system/etc/permissions/services.cn.google.xml`