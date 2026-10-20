# 墨听 APK 分发

本仓库**只存放安装包与更新清单，不包含任何源码**。

- `latest.json`：客户端检查更新时读取的唯一清单，请勿手工修改
- Releases：各版本 APK 附件（单个附件上限 2GB）

## 发布

由源码仓库的 `tools/build/publish-apk-release.sh` 自动维护：
上传 APK 到 Releases → 回写 `latest.json` 对应通道。

## 通道

| 通道 | 包名 | 说明 |
|---|---|---|
| release | `com.applecabal.njread` | 正式包 |
| debug | `com.applecabal.njread.debug` | 调试包 |
