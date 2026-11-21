<div align="center">
    <a href="https://www.youtube.com/@avencores/" target="_blank">
      <img src="https://github.com/user-attachments/assets/338bcd74-e3c3-4700-87ab-7985058bd17e" alt="YouTube" height="40">
    </a>
    <a href="https://t.me/avencoresyt" target="_blank">
      <img src="https://github.com/user-attachments/assets/939f8beb-a49a-48cf-89b9-d610ee5c4b26" alt="Telegram" height="40">
    </a>
    <a href="https://vk.ru/avencoresreuploads" target="_blank">
      <img src="https://github.com/user-attachments/assets/dc109dda-9045-4a06-95a5-3399f0e21dc4" alt="VK" height="40">
    </a>
    <a href="https://dzen.ru/avencores" target="_blank">
      <img src="https://github.com/user-attachments/assets/bd55f5cf-963c-4eb8-9029-7b80c8c11411" alt="Dzen" height="40">
    </a>
</div>

# 🔑 Open AG Patcher 中文说明
<p align="center">
  <a href="https://github.com/AvenCores/open-antigravity-patcher"><img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/badge/License-GPL--3.0-blue?style=for-the-badge" alt="GPL-3.0 许可证"></a>
  <a href="https://github.com/AvenCores/open-antigravity-patcher/releases/latest"><img src="https://img.shields.io/github/v/release/AvenCores/open-antigravity-patcher?style=for-the-badge" alt="上游最新版本"></a>
  <a href="https://github.com/moshoutegong/AvenCores-open-antigravity-patcher-CN/stargazers"><img src="https://img.shields.io/github/stars/moshoutegong/AvenCores-open-antigravity-patcher-CN?style=for-the-badge" alt="GitHub 星标"></a>
  <img src="https://img.shields.io/github/forks/moshoutegong/AvenCores-open-antigravity-patcher-CN?style=for-the-badge" alt="GitHub 复刻">
  <a href="https://github.com/moshoutegong/AvenCores-open-antigravity-patcher-CN/watchers">
  <img src="https://img.shields.io/github/watchers/moshoutegong/AvenCores-open-antigravity-patcher-CN?style=for-the-badge" alt="GitHub 关注者"></a>
  <a href="https://github.com/AvenCores/open-antigravity-patcher/releases"><img src="https://img.shields.io/github/downloads/AvenCores/open-antigravity-patcher/total?style=for-the-badge" alt="上游下载次数"></a>
  <a href="https://github.com/moshoutegong/AvenCores-open-antigravity-patcher-CN/pulls"><img src="https://img.shields.io/github/issues-pr/moshoutegong/AvenCores-open-antigravity-patcher-CN?style=for-the-badge" alt="GitHub 拉取请求"></a>
  <a href="https://github.com/moshoutegong/AvenCores-open-antigravity-patcher-CN/issues"><img src="https://img.shields.io/github/issues/moshoutegong/AvenCores-open-antigravity-patcher-CN?style=for-the-badge" alt="GitHub 议题"></a>
</p>

适用于 Antigravity 2.0、Antigravity IDE、Antigravity CLI 以及 VS Code 的 Google Antigravity 扩展的开源补丁工具：无需 VPN，也无需更改 Google 账号地区，即可解除本地地区限制。它是 [Antigravity IDE 在俄罗斯免 VPN、免修改 Google 账号地区工具](https://github.com/confeden/Antigravity)的开源替代方案。

> 本仓库为中文说明版本，原项目：[AvenCores/open-antigravity-patcher](https://github.com/AvenCores/open-antigravity-patcher)。以下功能与排障说明译自原 README。

![maxresdefault](https://i.ibb.co/s9Vh80CM/python-w-TPlox-Po-G4.png)

# 🎦 安装与故障排查视频教程

![maxresdefault](https://github.com/user-attachments/assets/54c4f1bd-01f5-4ee8-92d1-f7bbb910d079)

<div align="center">

[**在 YouTube 观看**](https://youtu.be/GyQVTxgt12E)

[**在 Rutube 观看**](https://rutube.ru/video/aba4484f8e0b5e67e966ff8229385f83/)

[**在 Dzen 观看**](https://dzen.ru/video/watch/6a7c430575822e0e4ba2970e)

[**在 VK Video 观看**](https://vkvideo.ru/video-234234162_456239108)

[**在 Telegram 观看**](https://t.me/avencoreschat/571689)

</div>

## ⚠️ HTTP 500 Internal Server Error 错误
如果在 Antigravity IDE 中发送请求时出现 HTTP 500 Internal Server Error，原文建议更换账号（优先使用 Antigravity IDE 官方支持地区的账号，或已购买付费订阅的账号）。原文提到，付费工具也无法解决此错误。

**错误示例**
```
Trajectory ID: 2669b09c-1d11-4620-9bfa-6ad1f0e26a88
Error: HTTP 500 Internal Server Error
Sherlog: 
TraceID: 0xd9ada64bcca3260c
Headers: {"Alt-Svc":["h3=\":443\"; ma=2592000,h3-29=\":443\"; ma=2592000"],"Content-Length":["109"],"Content-Type":["text/event-stream"],"Date":["Sat, 14 Mar 2026 13:51:24 GMT"],"Server":["ESF"],"Server-Timing":["gfet4t7; dur=423"],"Vary":["Origin","X-Origin","Referer"],"X-Cloudaicompanion-Trace-Id":["d9ada64bcca3260c"],"X-Content-Type-Options":["nosniff"],"X-Frame-Options":["SAMEORIGIN"],"X-Xss-Protection":["0"]}

{
  "error": {
    "code": 500,
    "message": "Internal error encountered.",
    "status": "INTERNAL"
  }
}
```

## ⚠️ HTTP 403 Forbidden / SUBSCRIPTION_REQUIRED (#3501) / Agent execution terminated due to error
如果 Antigravity IDE 或 CLI（`agy`）出现 `HTTP 403 Forbidden`，原因为 `SUBSCRIPTION_REQUIRED`，或提示 `You do not have a valid license of this product`、`Agent execution terminated due to error`，则问题不在本地补丁，也不是 `Eligibility Check` 界面。

此错误与 Google API 及用户账号状态有关，包括许可证、访问权限或 Google 服务端的授权检查。补丁工具仅修改 Antigravity/Antigravity CLI 的本地文件，无法为账号授予许可证，也无法改变 Google API 的响应，因此不能解决此错误。

**原文提供的处理方法：**
1. **更改 Google 账号地区**，或使用在 Antigravity 官方支持地区注册的账号。
2. **如果更改地区仍无效**，原文建议购买官方订阅。

**Google AI 订阅方案（以下价格、容量及额度为原文记录，未经当前核实，请以[官方页面](https://one.google.com/about/google-ai-plans/)及所在地区实际显示为准）：**

*   **Google AI Plus**
    *   **价格：** 每月 445 卢布
    *   **存储空间：** 400 GB
    *   **功能：** 使用 AI 工具提高工作效率，Gemini 使用额度提高至 2 倍*。
    *   [订阅 Plus](https://one.google.com/about/google-ai-plans/) | [查看方案权益](https://one.google.com/about/google-ai-plans/) *（附适用条件）*
*   **Google AI Pro**
    *   **价格：** 每月 1,790 卢布
    *   **存储空间：** 5 TB
    *   **功能：** Gemini 使用额度提高至 4 倍*，帮助完成更多工作。
    *   [订阅 Pro](https://one.google.com/about/google-ai-plans/) | [查看方案权益](https://one.google.com/about/google-ai-plans/) *（附适用条件）*
*   **Google AI Ultra**
    *   **价格：** 每月 6,990 卢布起
    *   **存储空间：** 20 TB 起
    *   **功能：** Gemini 使用额度提高至 20 倍*，加快工作流程。
    *   [订阅 Ultra](https://one.google.com/about/google-ai-plans/) | [查看方案权益](https://one.google.com/about/google-ai-plans/) *（附适用条件）*

**错误示例：**
```json
{
  "error": {
    "code": 403,
    "details": [
      {
        "@type": "type.googleapis.com/google.rpc.ErrorInfo",
        "domain": "cloudaicompanion.googleapis.com",
        "metadata": {
          "error_number": "1001",
          "uiMessage": "true"
        },
        "reason": "SUBSCRIPTION_REQUIRED"
      }
    ],
    "message": "You do not have a valid license of this product. Please contact your administrator to request a license. If you are not an enterprise user and believe you are receiving this message as an error, please try using the latest version and logging in again. (#3501)",
    "status": "PERMISSION_DENIED"
  }
}
```

## ⚠️ HTTP 400 Bad Request 错误
如果出现 `HTTP 400 Bad Request`，并提示 `User location is not supported for the API use`，表示 Google 将你的位置判定为不受支持的地区。

**原文提醒：** Google 可能检测到 VPN、代理或其他绕过限制的方式，并返回此错误。如果 IP 地址或其他会话参数被判定为可疑，访问可能被阻止。

**原文提供的处理方法：**
1. 应用补丁（**PATCH → `1`: Antigravity IDE patch**），在代码层面处理 `isGoogleInternal` 检查。
2. 如果已应用补丁，可尝试更换 Google 账号或其他 VPN。
3. 原文还列出了 **[Xbox DNS](https://xbox-dns.ru/)**、**[dns.malw.link](https://info.dns.malw.link/)**、**[GeoHide](https://dns.geohide.ru:8443/)**，这些是用于在电脑或路由器上处理地区限制的 DNS 服务。

**错误示例：**
```json
{
  "error": {
    "code": 400,
    "message": "User location is not supported for the API use.",
    "status": "FAILED_PRECONDITION"
  }
}
```

## ⚠️ HTTP 429 Too Many Requests / RESOURCE_EXHAUSTED 错误

向 Antigravity 发送提示词时，可能出现配额耗尽错误：

```
Error: HTTP 429 Too Many Requests
{
  "error": {
    "code": 429,
    "message": "Resource has been exhausted (e.g. check quota).",
    "status": "RESOURCE_EXHAUSTED"
  }
}
```

包含 Sherlog 的完整形式：
```
Error: HTTP 429 Too Many Requests
Sherlog:
TraceID: 0xe83b93ad455d1950
Headers: {"Alt-Svc":["h3=\":443\"; ma=2592000,h3-29=\":443\"; ma=2592000"],"Content-Length":["139"],"Content-Type":["text/event-stream"],"Date":["Sun, 06 Sep 2026 10:44:19 GMT"],"Server":["ESF"],"Server-Timing":["gfet4t7; dur=502"],"Vary":["Origin","X-Origin","Referer"],"X-Cloudaicompanion-Trace-Id":["e83b93ad455d1950"],"X-Content-Type-Options":["nosniff"],"X-Frame-Options":["SAMEORIGIN"],"X-Xss-Protection":["0"]}
```

**原文提供的处理方法：** 重置 Antigravity 数据目录（重新生成配置和令牌），然后按需从备份恢复对话。以下分别介绍 Windows、macOS 和 Linux 的操作。

> **Antigravity 与 Antigravity IDE：** Antigravity 2.0 的数据目录名为 `Antigravity`，Antigravity IDE 的数据目录名为 `Antigravity IDE`。请在以下命令中替换成实际目录名。下文统一以 `Antigravity` 为例。

### Windows 完整步骤

**1.** 完全退出 Antigravity（托盘 → `Quit` / 退出），并在任务管理器中确认没有 `Antigravity` 进程。

**2.** 打开 `%appdata%`（`Win+R` → 输入 `%appdata%` → `Enter`），将其中的 `Antigravity` 文件夹移动到安全位置，例如桌面：
```powershell
Move-Item "$env:APPDATA\Antigravity" "$env:USERPROFILE\Desktop\Antigravity-backup"
```

**3.** 启动 Antigravity，登录账号并发送测试提示词，检查 429 错误是否消失。

**4.** 如果恢复正常，关闭 Antigravity。

**5.** *（可选：恢复对话）* 仅恢复以下对话存储目录：
- `User\globalStorage`（对话数据）
- `User\workspaceStorage`

第 3 步启动时，Antigravity 已创建新的 `%appdata%\Antigravity` 数据目录。仅删除新目录中的以下两个文件夹，再从备份中复制回来：
```powershell
Remove-Item -Recurse -Force "$env:APPDATA\Antigravity\User\globalStorage"
Remove-Item -Recurse -Force "$env:APPDATA\Antigravity\User\workspaceStorage"

Copy-Item -Recurse "$env:USERPROFILE\Desktop\Antigravity-backup\User\globalStorage" "$env:APPDATA\Antigravity\User\"
Copy-Item -Recurse "$env:USERPROFILE\Desktop\Antigravity-backup\User\workspaceStorage" "$env:APPDATA\Antigravity\User\"
```

> ⚠️ **不要复制**备份中的 `settings.json`，否则会恢复旧的问题配置。

**6.** 启动 Antigravity，检查对话并发送提示词。确认一切正常后，可删除备份：
```powershell
Remove-Item -Recurse -Force "$env:USERPROFILE\Desktop\Antigravity-backup"
```

### macOS 完整步骤

**1.** 完全退出 Antigravity（`Cmd+Q`），确认 Dock 图标下方的小圆点已消失。

**2.** 将数据目录移动到安全位置：
```bash
mv ~/Library/Application\ Support/Antigravity ~/Desktop/Antigravity-backup
```

**3.** 启动 Antigravity，登录并发送测试提示词，检查 429 错误是否消失。

**4.** 如果恢复正常，关闭 Antigravity（`Cmd+Q`）。

**5.** *（可选：恢复对话）* 第 3 步启动时已生成新的 `~/Library/Application Support/Antigravity` 数据目录。仅删除其中的对话存储目录，再从备份复制回来：
```bash
rm -rf ~/Library/Application\ Support/Antigravity/User/globalStorage
rm -rf ~/Library/Application\ Support/Antigravity/User/workspaceStorage

cp -a ~/Desktop/Antigravity-backup/User/globalStorage ~/Library/Application\ Support/Antigravity/User/
cp -a ~/Desktop/Antigravity-backup/User/workspaceStorage ~/Library/Application\ Support/Antigravity/User/
```

> ⚠️ **不要复制**备份中的 `settings.json`，否则会恢复旧的问题配置。

**6.** 启动 Antigravity，检查对话并发送提示词。确认一切正常后，可删除备份：
```bash
rm -rf ~/Desktop/Antigravity-backup
```

### Linux 完整步骤

Linux 数据目录为 `${XDG_CONFIG_HOME:-~/.config}/Antigravity`（通常为 `~/.config/Antigravity`）。

**1.** 完全退出 Antigravity：
```bash
pkill -f -i antigravity; sleep 2; pgrep -a -i antigravity || echo "closed"
```

**2.** 将数据目录移动到安全位置：
```bash
# 默认路径
mv ~/.config/Antigravity ~/Antigravity-backup

# 如果设置了 XDG_CONFIG_HOME：
# mv "${XDG_CONFIG_HOME:-$HOME/.config}/Antigravity" ~/Antigravity-backup
ls -d ~/Antigravity-backup
```

**3.** 启动 Antigravity，登录并发送测试提示词，检查 429 错误是否消失。

**4.** 如果恢复正常，关闭 Antigravity（见第 1 步）。

**5.** *（可选：恢复对话）* 第 3 步启动时已生成新的 `~/.config/Antigravity` 数据目录。仅删除其中的对话存储目录，再从备份复制回来：
```bash
rm -rf ~/.config/Antigravity/User/globalStorage
rm -rf ~/.config/Antigravity/User/workspaceStorage

cp -a ~/Antigravity-backup/User/globalStorage ~/.config/Antigravity/User/
cp -a ~/Antigravity-backup/User/workspaceStorage ~/.config/Antigravity/User/
```

> ⚠️ **不要复制**备份中的 `settings.json`，否则会恢复旧的问题配置。

**6.** 启动 Antigravity，检查对话并发送提示词。确认一切正常后，可删除备份：
```bash
rm -rf ~/Antigravity-backup
```

### 原文对该方法的解释

移动数据目录后，Antigravity 会从头创建配置并生成新的令牌。原文认为，这可能清除与旧配额状态相关的本地绑定；实际服务端配额仍由 Google 决定。

### 已应用补丁的用户须知

补丁修改的是已安装应用内的 `main.js`（macOS 为 `.app` 包内文件）。移动用户数据目录**不会影响该文件**，通常无需重新应用文件补丁。

重置的只有 `settings.json` 中的运行时兼容处理。如果重置后出现问题，再运行一次补丁工具（菜单第 1 项）。工具会检测到 `main.js` 已打补丁，仅应用设置层面的兼容处理。

## ⚠️ Antigravity CLI 许可证错误 (#3501)
如果 Antigravity CLI（`agy`）提示 `You do not have a valid license of this product`，则问题不在本地补丁，也不是 `Eligibility Check` 界面。

此错误与 Google API 及用户账号状态有关，包括许可证、访问权限或 Google 服务端的授权检查。补丁工具仅修改 Antigravity/Antigravity CLI 的本地文件，无法为账号授予许可证，也无法改变 Google API 的响应，因此不能解决此错误。

**错误示例：**
```text
⚠ You do not have a valid license of this product. Please contact your administrator to request a license. If you are
not an enterprise user and believe you are receiving this message as an error, please try using the latest version and
logging in again. (#3501)
Error ID: b2c1d9edcaac4fd5ac5766de06c2253b
Trajectory ID: d3ee4302-4213-40f9-9ac5-42e83e38a5ce
```

## ⚠️ 补丁错误："✗ isGoogleInternal -> true (auth) — pattern not found"

应用补丁（PATCH → `1`: Antigravity IDE patch）时，如果出现：

```text
✗ isGoogleInternal -> true (auth) — pattern not found
```

表示工具在准备修改的 `main.js` 中未找到预期的 `isGoogleInternal` 模式。

**原文指出，这种情况几乎总是因为工具误选了与 Antigravity IDE 无关的 `main.js` 文件。**

### 处理方法

1. 在补丁工具主菜单中检查识别到的 `main.js` 路径（通常会在应用补丁前显示）。
2. 确认路径指向 Antigravity IDE 的实际文件，例如：
   - Windows: `%LOCALAPPDATA%\Programs\Antigravity IDE\resources\app\out\main.js`
   - Linux: `/usr/share/antigravity-ide/resources/app/out/main.js`
   - macOS: `/Applications/Antigravity IDE.app/Contents/Resources/app/out/main.js`
3. 如果路径指向其他文件（例如另一个 Electron 应用或脚本当前目录内的 `main.js`），选择 **TOOLS → `11` (Select custom path)**，手动指定正确的 Antigravity IDE 目录。
4. 确认补丁工具的工作目录中没有其他 `main.js`，否则工具可能优先选中它（搜索从当前目录开始）。

> **说明：** 如果当前目录包含其他项目的 `main.js`，请将脚本移到其他目录，或通过命令行参数明确指定 Antigravity IDE 路径：
>
> ```bash
> python main.py "C:\Users\<username>\AppData\Local\Programs\Antigravity IDE"
> ```

## 📚 更多错误说明
如需进一步了解 HTTP 错误类型和诊断方法，可参考：
- [5xx 服务器错误完整指南（英文）](https://komodor.com/learn/5xx-server-errors-the-complete-guide/)——详细介绍服务器错误。

## 🌟 功能特点
- 在标准路径和 Windows 注册表中自动查找 Antigravity 2.0、Antigravity IDE、Antigravity CLI（`agy`）以及 VS Code 的 Google Antigravity 扩展。
- **检查更新**：启动时自动检查新版本，也可通过菜单手动检查（TOOLS → `9`）。
- **Antigravity CLI 补丁**：通过 x86-64 和 ARM64 字节特征，在 `agy`/`agy.exe` Go 二进制文件的机器码层面处理资格检查，移除“Eligibility Check”界面，支持备份和还原。
- **Antigravity Manager（`language_server`）补丁**：通过 x86-64 和 ARM64 字节特征修改已编译的后端二进制文件，将授权检查设为 `hasValidAuth=true`，支持备份和还原。
- **VS Code 的 Google Antigravity 扩展补丁**：向 `google.google-antigravity` 扩展的 `extension.js` 注入防止重复下载的检查，并关闭发布渠道变更检查（`isChannelChanged -> false`），避免已下载或已修改的二进制文件被覆盖。此外，可对 `~/.gemini/bin/antigravity` 应用 agy 补丁。
- 支持 Linux：搜索 `/usr/share/antigravity-ide`，通过 `dpkg`、`rpm` 和 `package.json` 识别版本。
- 支持 macOS：在 `/Applications` 和 `~/Applications` 中搜索 `.app`，修改 `main.js` 后自动进行 ad-hoc 重新签名。
- 修改前创建备份。
- **POSIX 平台原子替换二进制文件**：Linux/macOS 上的 `agy` 和 `language_server` 通过同目录临时文件（`tempfile.mkstemp`，O_EXCL）及 `os.replace` 写入。正在运行的进程不会因文件被占用而阻止补丁（避免 `ETXTBSY` / `Permission denied`）；保留原有权限（包括 `+x`）、所有者和用户组；出错时删除临时文件，并拒绝修改符号链接。公共实现位于 `source/patcher/utils/atomic.py`。
- 通过简单菜单应用或还原补丁。
- 支持 `resources/app/out/main.js` 和 `resources/app/main.js` 路径。
- 彩色输出，并尝试自动提升权限（Windows 使用 UAC，Linux 提示使用 `sudo`）。
- 应用补丁前检查 Antigravity IDE 最低版本（>= `2.1.1`）。
- 通过 Windows 注册表、Linux 包管理器或 macOS 的 `package.json` 识别 Antigravity IDE 版本。
- 检测已应用的补丁，并提供重新应用选项。

## 🚀 使用方法
1. 关闭 Antigravity IDE 或 Antigravity 2.0。
2. 以管理员身份运行补丁工具（需要时，脚本会请求提升权限）。
3. 在菜单中选择所需操作（保留英文菜单名称，便于对照程序）：

| 菜单项 | 说明 |
|---|---|
| **PATCH** | |
| `1` Antigravity IDE patch | 修改 Antigravity IDE 的 `main.js`，处理地区限制 |
| `2` Antigravity 2.0 patch | 修改 `language_server` 二进制文件（Antigravity Manager） |
| `3` Antigravity CLI (agy) patch | 修改 `agy`/`agy.exe` 二进制文件，解锁 agy 工具 |
| `4` Antigravity VS Code Patch | 修改 `google.google-antigravity` 的 `extension.js` 及 `~/.gemini/bin/antigravity`（需先安装并修改 Antigravity 2.0） |
| **RESTORE** | |
| `5` Antigravity IDE | 从备份恢复 Antigravity IDE 的原始 `main.js` |
| `6` Antigravity 2.0 | 从备份恢复原始 `language_server` |
| `7` Antigravity CLI | 从备份恢复原始 `agy`/`agy.exe` |
| `8` Antigravity VS Code extension | 从备份恢复原始 `extension.js` 及 `~/.gemini/bin` 二进制文件 |
| **TOOLS** | |
| `9` Check for updates | 检查 GitHub 上的新版本 |
| `10` Open GitHub repository | 在浏览器中打开项目页面 |
| `11` Select custom path | 手动选择应用目录或文件路径（IDE / 2.0 / CLI / VS Code 扩展） |
| `12` About program | 显示程序与作者信息 |
| **`0` Exit** | 退出补丁工具 |

从源码运行（先进入 `source` 目录并安装依赖，详见[构建说明](#build)）：
```bash
python main.py
```

指定路径运行（适用于 Antigravity IDE、Antigravity 2.0 或 Antigravity CLI）：
```bash
# Windows
python main.py "C:\\Users\\<username>\\AppData\\Local\\Programs\\Antigravity IDE"
python main.py "C:\\Users\\<username>\\AppData\\Local\\Programs\\Antigravity\\resources\\bin\\language_server.exe"
python main.py "C:\\Users\\<username>\\AppData\\Local\\agy\\bin\\agy.exe"

# Linux
python main.py /usr/share/antigravity-ide
python main.py /opt/Antigravity/resources/bin/language_server
python main.py /usr/local/bin/agy

# macOS
python3 main.py /Applications/Antigravity\ IDE.app
python3 main.py /Applications/Antigravity.app
python3 main.py /usr/local/bin/agy
```

如果 `main.js` 或 `language_server` 与脚本位于同一目录，无需指定路径，工具会自动查找。

> **macOS：** 如果 `Antigravity IDE.app` 位于 `/Applications`，写入需要 `sudo`（脚本会提示重新运行）；安装在 `~/Applications` 或用户目录时通常不需要。成功应用补丁后，`.app` 会自动进行 ad-hoc 重新签名（`/usr/bin/codesign --force --deep --sign -`），否则启用 Hardened Runtime 的 Electron 应用无法在 macOS 启动。扫描已签名的 Mach-O 文件时直接读入内存（不使用 `mmap`），避免内核在检查已修改文件时以 CODESIGNING SIGKILL 终止进程。移除 `com.apple.quarantine` 使用系统自带的 `/usr/bin/xattr`，无需额外 Python 包。

### 🍎 macOS 使用方法

原文所述的官方发行版仅提供 Windows 和 Linux 预编译文件，未提供 macOS 版本。macOS 用户可直接运行源码，或自行构建可执行文件。

#### 方案一：从源码运行（推荐）
1. 进入 `source` 目录，创建并激活虚拟环境，然后安装依赖：
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```
2. 完全退出 Antigravity 2.0 或 Antigravity IDE。
3. 启动补丁工具，并指定应用路径：
   ```bash
   # Antigravity IDE
   python3 main.py "/Applications/Antigravity IDE.app"
   
   # Antigravity 2.0
   python3 main.py "/Applications/Antigravity.app"
   ```
   *说明：如果应用位于 `/Applications`，脚本会自动请求提升权限（`sudo`）以写入文件。*

#### 方案二：自行构建二进制文件
如需可执行文件，可按照[🛠️ 构建](#build)一节自行构建。

构建成功后，通过终端运行生成的文件：
```bash
cd dist
chmod +x Open_AG_Patcher_macOS
sudo ./Open_AG_Patcher_macOS
```
如果 macOS 阻止运行生成的文件，原文提供了以下移除 quarantine 属性的命令：
```bash
xattr -dr com.apple.quarantine Open_AG_Patcher_macOS
```

#### 菜单选择
按目标选择：
- **PATCH → `1`**（Antigravity IDE patch）：`Antigravity IDE.app`
- **PATCH → `2`**（Antigravity 2.0 patch）：`Antigravity.app`（language_server 后端）
- **PATCH → `3`**（Antigravity CLI (agy) patch）：`agy` 二进制文件（如已安装）
- **PATCH → `4`**（Antigravity VS Code Patch）：VS Code 中的 `google.google-antigravity` 扩展
- **RESTORE → `5`**、`6`、`7` 或 `8`：从备份还原

对于 `Antigravity.app`，工具通常会自动找到：
```text
/Applications/Antigravity.app
```
如果自动查找失败，选择 **TOOLS → `11`**（Select custom path），并指定以下路径之一：
```text
/Applications/Antigravity.app
/Applications/Antigravity IDE.app
```

#### 检查签名
应用补丁后，`.app` 会自动使用 ad-hoc 签名重新签名。可使用以下命令检查：
```bash
codesign -dv /Applications/Antigravity.app 2>&1 | grep Signature
```
预期输出：
```text
Signature=adhoc
```

## ❓ 具体修改内容

### Antigravity IDE 补丁

工具修改 `main.js`，处理 `isGoogleInternal` 检查。可通过备份文件（`main.js.bak`）还原。

### `resetIsTierGCPTos(),this.XXX.isGoogleInternal` → `resetIsTierGCPTos(),true`
将授权服务中 `resetIsTierGCPTos()` 调用后的 `isGoogleInternal` 检查替换为固定的 `true`，启用 Google 内部访问分支。应用补丁后，自动清理 VS Code 缓存目录（`CachedData` 和 `Code Cache/js`），让 IDE 重新编译修改后的 JS 代码。


### Antigravity Manager（language_server）补丁

Antigravity Manager（`language_server` 或 `language_server.exe`）是 Antigravity 2.0 内部启动的后端服务，默认要求通过 Google 端的授权和许可证检查。

工具通过 `MultiGate` 类，按字节特征直接修改已编译的 `language_server` 二进制文件，支持两种架构：
- **x86-64**（Intel Mac / Windows / Linux x64）：将 `cmp byte ptr [rax + 8], 0` 替换为 `mov byte ptr [rax + 8], 1`，并补上 `nop`（`\xc6\x40\x08\x01\x90\x90`）。
- **ARM64**（Linux arm64 / Apple Silicon macOS）：将 `ldrb w3, [x0, #8] ; tbz w3, #0, skip` 序列（考虑前面一条或两条准备指令）替换为 `mov w3, #1 ; strb w3, [x0, #8]`（`\x23\x00\x80\x52\x03\x20\x00\x39`）。

修改后，返回值 `hasValidAuth` 被固定为 `true`，从而解除本地阻止。
可通过 **RESTORE → `6`** 从 `.agybak` 恢复原始二进制文件。
POSIX 平台采用与 `agy` 相同的原子写入方式（临时文件 + `os.replace`，保留 `+x` 和所有者）；正在运行的 `language_server` 不会阻止补丁。

### Antigravity CLI（agy）补丁

Antigravity CLI 是独立的 Go 二进制程序（Windows 为 `agy.exe`，Linux/macOS 为 `agy`），会根据服务端响应显示“Eligibility Check”界面并生成“Account ineligible”错误。由于它是编译后的二进制文件而非 JS，工具通过 `MultiGate` 在**机器码层面**按唯一字节特征修改，支持 **x86-64**（Windows / Linux x64 / Intel Mac）和 **ARM64**（Windows ARM64 / Linux arm64 / Apple Silicon macOS）。

工具针对**一类检查关卡**进行修改，使错误构造前的外层检查无法进入错误分支：

#### Gate 1：“Eligibility Check”界面

##### x86-64
1. 扫描二进制文件，查找关卡检查的唯一特征：
   ```asm
   test rax, rax              ; 48 85 c0            <-- 授权结果是否为 nil？
   je  eligible               ; 0f 84 xx xx xx xx   <-- 为 nil → 通过
   cmp byte ptr [rax+8], 0   ; 80 78 08 00         <-- 检查资格标志
   jne eligible               ; 0f 85 xx xx xx xx   <-- 标志非 0 → 通过
   call failure_builder       ; e8 xx xx xx xx      <-- 失败：构造错误
   ```
2. 将 `cmp byte ptr [rax+8], 0` 替换为 `test rax,rax` + `NOP`（`48 85 c0 90`）。由于此处 `rax` 保证非零，`jne` 总会跳转至“eligible”分支。

##### ARM64
1. 在原文所述的原生 arm64 构建中，错误构造前的外层检查如下：
   ```asm
   cbnz x1, error            ; xx xx xx b5     <-- x1 非 0 → 失败
   cbz  x0, eligible         ; xx xx xx b4     <-- x0 为 0 → 通过
   ldrb w1, [x0, #8]        ; 01 20 40 39     <-- 读取资格标志
   tbnz w1, #0, eligible    ; xx xx xx 37     <-- 第 0 位非 0 → 通过
   bl   failure_builder      ; xx xx xx 97     <-- 失败：构造错误
   ```
2. 将资格标志加载指令 `ldrb w1,[x0,#8]` 替换为 `mov w1,#1`（`21 00 80 52`），使现有 `tbnz` 总是选择“eligible”分支。`MultiGate` 自动选择 x64 或 arm64 特征。严格的统一 ARM64 关卡覆盖两种已知尾部：经典形式（`x0`/`x1`/`x2` → `[sp,#0x90]`/`[sp,#0x60]`/`[sp,#0x80]`）以及 macOS 构建形式（`x0`/`x1`/`x2`/`x3` → `[sp,#0x98]`/`[sp,#0x60]`/`[sp,#0x88]`/`[sp,#0x58]`）。CLI 1.2.7 起，重新编译的检查不再包含外层 `cbnz`（`cbz x0` → `ldrb w4,[x0,#8]` → `tbnz w4,#0` → `ldp x4,x5,[x0,#0x48]`），由独立关卡 `eligibility screen off (arm64, w4)` 覆盖，替换为 `mov w4,#1`（`24 00 80 52`）。界面函数还有内联检查（`cbnz x1` → `cbz x0` → `ldrb w2,[x0,#8]` → `tbnz w2,#0` → `bl`），由 `eligibility screen off (arm64, w2)` 覆盖，替换为 `mov w2,#1`（`22 00 80 52`）；否则即使修改 w4，仍会显示 `Eligibility check failed:`。`MultiGate` 使用 `resolve_all` 收集**所有**子关卡的匹配，因此 1.2.7 的两个位置都会修改。`test-agy/test_cli_releases.py` 会下载最新发行版的所有归档，自动测试兼容性。

#### 通用步骤
3. 写入前创建 `agy.exe.agybak` 备份（POSIX 为 `agy.agybak`）。如果应用自动更新导致现有备份过时，工具会自动更新备份，不保留过期副本。
4. Linux/macOS 使用原子写入：在同目录创建临时文件（`tempfile.mkstemp`，O_EXCL），写入新字节并执行 `fsync`，随后通过 `os.replace` 替换目标，保留原始权限、所有者和用户组。正在运行的 `agy` 继续使用旧 inode，后续启动使用新文件，因此不会阻止补丁。Windows 则直接写入目标文件。
5. macOS 修改后二进制文件会进行 ad-hoc 重新签名（与 `.app` 相同）。

**补丁安全检查：**
- 如果未找到字节特征（未知或不支持的版本），工具会**拒绝修改**并提示 `signature not found (unsupported version?)`。
- 写入前验证每个补丁：偏移量不得为负，不能超出文件边界，也不能改变文件大小。
- 禁止修改符号链接；目标必须是普通文件，否则拒绝写入。
- 如果特征出现多次（Go 可能为同一函数编译出多个实例），工具会修改**所有**匹配位置，因为它们在机器码层面相同。
- 通过 **RESTORE → `7`**（Antigravity CLI）从 `.agybak` 还原。

> **平台说明：** x86-64 特征已在 Windows 和 Intel macOS 上验证，ARM64 特征已在 Apple Silicon macOS 上验证。查找逻辑跨平台搜索二进制文件（`PATH`、Windows 的 scoop，以及 POSIX 的 `/usr/local/bin`、`/opt/antigravity/bin`、`~/.local/bin`）。Linux 的 `agy` 可能采用不同编译方式，导致特征不匹配；此时工具只报告问题，不修改文件。

### Google Antigravity（VS Code）扩展补丁

> **⚠️ 重要：** 修改 VS Code 扩展（`PATCH → 4`）前，必须先安装并修改 Antigravity 2.0（`PATCH → 2`，即 `language_server` 补丁）。请先安装 Antigravity 2.0、应用补丁，再修改 VS Code 中的 `google.google-antigravity` 扩展。

VS Code 的 `google.google-antigravity` 扩展每次启动都会检查后端二进制版本，并从 Google 发布服务器重新下载。工具会对扩展的 `extension.js` 进行两处修改：

#### 第一部分：防止重复下载

在 `outputChannel.appendLine('[INSTALL] Checking Antigravity releases...')` 之后注入代码，检查已下载的二进制文件（`targetPathOverride` 或 `~/.gemini/bin`）。如果找到文件，就**立即返回其路径**，跳过版本检查和重新下载：

```js
{const __primary=options.targetPathOverride||getInstalledTargetPath();
const __candidates=[__primary,
(0,path_1.join)((0,path_1.dirname)(__primary),'antigravity'+((0,path_1.extname)(__primary)||''))];
for(const __p of __candidates){if(__p&&await pathExists(__p)){
outputChannel.appendLine('[INSTALL] Existing binary found at '+__p+'. Skipping version check and re-download.');return __p;}}}
```

插入位置使用灵活的正则表达式查找，匹配**完整的** `outputChannel.appendLine('...');` 调用，兼容不同引号和空格，并严格匹配到调用的右括号，确保代码插在调用之后。

#### 第二部分：关闭发布渠道变更检查

```js
// 修改前：
const isChannelChanged = manifestFetched && lastInstalledUrl !== releaseBaseUrl;
// 修改后：
const isChannelChanged = false;
```

否则，扩展可能认为发布渠道已变更，强制重新下载二进制文件并覆盖已打补丁的版本。

#### 附加操作：修改下载的二进制文件

修改 `extension.js` 后，工具会询问是否对扩展下载的 `~/.gemini/bin/antigravity`（或 `~/.gemini/bin/agy`）应用上文的 agy 补丁，因为其中包含相同的资格检查。

**细节：**
- 备份为原文件旁的 `extension.js.vscodebak`；过期备份会自动更新。
- 通过注入代码和 `const isChannelChanged = false;` 检测是否已应用补丁。
- 还原：**RESTORE → `8`** 从 `.vscodebak` 恢复 `extension.js`，并询问是否从 `.agybak` 恢复 `~/.gemini/bin` 中的二进制文件。
- 应用补丁后，需要重新加载 VS Code 窗口（**Developer: Reload Window**）。
- 扩展查找目录：`~/.vscode/extensions`、`~/.vscode-insiders/extensions`、`~/.vscode-oss/extensions`、`~/.vscode-server/extensions`、`~/.vscode-server-insiders/extensions`，或环境变量 `VSCODE_EXTENSIONS` 指定的目录。存在多个版本时，按 mtime（修改时间）选择最新项。

## 🔍 文件查找逻辑

工具按以下顺序查找 `main.js`：

1. 命令行参数（目录路径或 `main.js` 文件路径）。
2. 当前目录（`./main.js`）。
3. 自动搜索标准路径：
   - **Windows:**
     - `%LOCALAPPDATA%\Programs\Antigravity IDE`
   - **Linux:**
     - `/usr/share/antigravity-ide`
     - `/opt/Antigravity IDE`
     - `/opt/Antigravity IDE/resources/app/out`
   - **macOS:**
     - `/Applications/Antigravity IDE.app/Contents/Resources/app`
     - `~/Applications/Antigravity IDE.app/Contents/Resources/app`
4. Windows 注册表：`HKCU` 和 `HKLM` 下 `SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall\` 中的 `{AA73B3E3-C6C8-45C8-B1DC-4AE56C751432}_is1` 项。

在找到的目录内检查以下路径：
- `resources/app/out/main.js`
- `resources/app/main.js`
- `out/main.js` (macOS)
- `main.js`（直接指定文件路径时）

macOS 也可直接传入 `.app` 包路径，脚本会自动解析为 `Contents/Resources/app/out/main.js`。

### 查找 Antigravity CLI（`agy`）

工具通过 `PATH` 和标准目录查找 `agy`（Windows 为 `agy.exe`），不依赖固定安装位置或版本：

1. 命令行参数，或 **TOOLS → `11` → `3`**（指定 `agy`/`agy.exe` 文件或所在目录）。
2. `PATH` (`shutil.which("agy")`).
3. 标准目录：
   - **Windows：** `%LOCALAPPDATA%`、`%PROGRAMFILES%`、`%PROGRAMFILES(X86)%`、`%ProgramData%`、`%APPDATA%`（以及 `Programs` 子目录），还有 scoop（`%USERPROFILE%\scoop\apps`、`%SCOOP%\apps`）。匹配模式：`agy/bin/agy.exe`、`agy/*/bin/agy.exe`（scoop 版本目录）、`agy*/agy.exe`。
   - **Linux/macOS:** `/usr/local/bin`, `/usr/bin`, `/opt/antigravity/bin`, `/opt/antigravity`, `~/.local/bin`, `~/bin`.

如果找到多个副本（例如 scoop 安装了多个版本），按 mtime 选择最新项。

### 查找 Google Antigravity（VS Code）扩展

`google.google-antigravity` 扩展的 `extension.js` 会在以下目录中查找（优先使用环境变量 `VSCODE_EXTENSIONS` 指定的目录）：

1. 命令行参数，或 **TOOLS → `11` → `4`**（`extension.js` 路径、`google.google-antigravity-*` 扩展目录，或 `extensions` 根目录）。
2. `~/.vscode/extensions`
3. `~/.vscode-insiders/extensions`
4. `~/.vscode-oss/extensions`
5. `~/.vscode-server/extensions`（远程服务器）
6. `~/.vscode-server-insiders/extensions`

在扩展目录中按 `google.google-antigravity-*` 匹配文件夹；存在多个版本时按 mtime 选择最新项。目标文件为扩展根目录中的 `extension.js`。

### 查找 `~/.gemini/bin` 二进制文件

扩展下载的二进制文件（仅用于 **PATCH → `4`**）位于 `~/.gemini/bin`：Windows 为 `antigravity.exe`/`agy.exe`，POSIX 为 `antigravity`/`agy`。如果文件不存在且扩展从未启动，工具会提示先在 VS Code 中运行一次扩展，让它下载二进制文件。

## 🔎 识别 Antigravity IDE 版本

| 平台 | 版本识别方式 |
|---|---|
| **Windows** | 注册表 `{AA73B3E3-...}_is1` 项中的 `DisplayVersion` |
| **Linux (deb)** | `dpkg-query -W antigravity-ide` |
| **Linux (rpm)** | `rpm -q --queryformat %{VERSION} antigravity-ide` |
| **Linux (portable/snap/flatpak)** | `main.js` 旁的 `package.json` |
| **macOS** | `Antigravity IDE.app/Contents/Resources/app/` 内的 `package.json` |

如果无法识别版本，工具会询问是否跳过检查继续运行。如果版本低于 `2.1.1`，会显示警告并提供选择。

## 🔒 检测已应用的补丁

修改前，脚本通过以下两个特征判断文件是否已打补丁：
- 不再包含 `if(this.X.isGoogleInternal)`（已替换为 `if(true)`）。
- 不再包含未修改的 `isGoogleInternal`（逗号表达式形式的授权检查）。

## 🛡️ 权限提升

- **Windows：** 使用 `ShellExecuteW` 和 `runas` 自动发起 UAC 请求，支持含空格的路径。
- **Linux：** 非 root 运行时，会询问是否通过 `sudo` 重新运行（`os.execvp`）。拒绝后仍继续，但提示可能发生写入错误。运行时兼容设置写入原始用户（`SUDO_USER`/`SUDO_UID`）的 `settings.json`，不会写入 `/root/.config/...`。
- **macOS：** 使用相同的 POSIX 逻辑，非 root 运行时提示使用 `sudo`。对于 `~/Applications/Antigravity IDE.app`，目录通常已可写，可回答 `n`；对于 `/Applications/Antigravity IDE.app`，通常需要同意提升权限。使用 `sudo` 时仍读取原始用户主目录中的 `settings.json`。

## 🍎 macOS 特别说明

### 应用补丁后重新签名 `.app`

修改已签名 `.app` 内的任意文件都会破坏代码签名。启用 Hardened Runtime 的 Electron 应用（包括 Antigravity IDE）随后可能**无法启动**，甚至还未显示 Gatekeeper 对话框就已退出。

为使 `.app` 能继续运行，脚本会在 `do_patch` 和 `do_restore` 后自动执行：

```bash
codesign --force --deep --sign - /path/to/Antigravity\ IDE.app
xattr -dr com.apple.quarantine /path/to/Antigravity\ IDE.app
```

`--sign -` 表示 ad-hoc 签名（无 Developer ID），足以在本地运行，无需公证（Notarization）。

需要安装 `codesign`，它随 **Xcode Command Line Tools** 提供：
```bash
xcode-select --install
```

### 应用补丁时出现 "Operation not permitted"

如果遇到 `[!] Backup error: [Errno 1] Operation not permitted: '/Applications/Antigravity IDE.app/Contents/Resources/app/out/main.js.bak'`：

1. 为终端开启完全磁盘访问权限：**系统设置 → 隐私与安全性 → 完全磁盘访问权限**（System Settings → Privacy & Security → Full Disk Access）。
2. 原文提供以下命令移除应用的隔离属性：
   ```bash
   sudo xattr -rd com.apple.quarantine /path/to/Antigravity\ IDE.app
   ```

### 应用补丁后无法启动

1. 确认 `codesign` 可用：`which codesign`。
2. 检查 `.app` 是否已重新签名：`codesign -dv /Applications/Antigravity\ IDE.app 2>&1 | grep Signature`，应看到 `Signature=adhoc`。
3. 如果 macOS 仍阻止运行，原文建议检查**系统设置 → 隐私与安全性**底部的“仍要打开”选项。

## ⚙️ 运行要求

- **Python** 3.x
- **依赖：** `packaging`（用于版本比较）
- **操作系统：**
  - **Windows：** 完整支持通过注册表自动查找，以及 UAC 权限提升。
  - **Linux：** 自动搜索 `/usr/share/antigravity-ide`，通过 `dpkg`/`rpm`/`package.json` 识别版本，支持 sudo 权限提升。
  - **macOS：** 自动搜索 `/Applications/Antigravity IDE.app` 和 `~/Applications/Antigravity IDE.app`，通过 `package.json` 识别版本，使用 `codesign`（Xcode Command Line Tools）进行 ad-hoc 重新签名。
- **Antigravity 2.0 最低版本：** `2.5.0`
- **Antigravity IDE 最低版本：** `2.1.1`
- **原文列出的支持版本：** Antigravity 2.0 为 `2.3.0` 及以上，IDE 为 `2.1.1` 及以上（原文对 2.0 的最低版本与支持范围表述不一致，使用时以工具实际检查为准）。

<a id="build"></a>

## 🛠️ 构建

建议使用虚拟环境构建可执行文件：

1. **创建并激活虚拟环境：**
   * **Windows:**
     ```bash
     cd source
     python -m venv .venv
     .venv\Scripts\activate
     ```
   * **Linux / macOS:**
     ```bash
     cd source
     python3 -m venv .venv
     source .venv/bin/activate
     ```

2. **安装依赖：**
   ```bash
   pip install -r requirements.txt
   ```

3. **使用 PyInstaller 构建：**
   * **Windows:**
     ```bash
     pyinstaller --onefile --uac-admin --icon=icon.ico --name="Open_AG_Patcher_Windows" --noupx --clean --version-file=version.txt main.py
     ```
   * **Linux:**
     ```bash
     pyinstaller --onefile --icon=icon.ico --name="Open_AG_Patcher_Linux" --hidden-import=packaging --hidden-import=packaging.version --hidden-import=packaging.specifiers --hidden-import=packaging.requirements main.py
     ```
   * **macOS (Universal2):**
     ```bash
     pyinstaller --onefile --name="Open_AG_Patcher_macOS" --target-arch universal2 --hidden-import=packaging --hidden-import=packaging.version --hidden-import=packaging.specifiers --hidden-import=packaging.requirements main.py
     ```

## 项目结构

- `source/main.py`：补丁工具入口，检查权限并启动 CLI。
- `source/patcher/`：采用模块化架构的主要源码：
  - `constants.py`：全局常量、正则表达式与版本信息。
  - `cli.py`：控制台用户界面、菜单和输入处理。
  - `utils/`：系统工具，包括控制台颜色、管理员权限、POSIX 权限、文件哈希，以及二进制文件原子替换（`atomic.py`）。
  - `ide/`：Antigravity IDE 的查找和补丁逻辑（`main.js`）。
  - `agy/`：Antigravity CLI（`agy`/`agy.exe`）的查找及字节特征补丁逻辑。
  - `manager/`：Antigravity Manager（`language_server`/`language_server.exe`）的查找及字节特征补丁逻辑。
  - `vscode/`：VS Code 的 `google.google-antigravity` 扩展（`extension.js`）及其下载到 `~/.gemini/bin` 的二进制文件的查找和补丁逻辑。
- `source/requirements.txt`：构建与运行依赖。
- `source/build.txt`：各操作系统的构建命令示例。
- `source/icon.ico`：`exe`/`app` 图标。

# 📜 许可证与署名

本项目采用 GPL-3.0 许可证，完整文本见 [`LICENSE`](LICENSE)。

本项目的部分修改与方案基于 MIT 许可的 [eligibility-antigravity-patcher](https://github.com/QNIX-Dev/eligibility-antigravity-patcher) 仓库。所有集成和修改均保留版权信息并注明原始来源。

---
# 💰 支持原作者
+ **SBER**: `2202 2050 1464 4675`
