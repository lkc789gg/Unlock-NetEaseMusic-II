## 🎵 Unlock-NetEaseMusic-II

**Unlock-NetEaseMusic-II** 让海外用户解锁网易云音乐的灰色歌曲！

👉 简易快速上手

👉 无需本地部署

👉 全自动 GitHub Actions，每天自动运行

---

## 🚀 快速开始

### 1. Fork 仓库

- 点击页面右上角 **Fork**，复制项目到自己的 GitHub 账号。
- 喜欢的话点个 ⭐ 。

### 2. 获取 `MUSIC_U`

- 打开 [网易云音乐](https://music.163.com/) (推荐使用 Chrome 浏览器)。
- 登录账号，按 `F12` 打开开发者工具。
- 进入「Application」 →「Cookies」→ `https://music.163.com`。
- 找到 `MUSIC_U`，复制它的值。

### 3. 修改 `auto_login.py`

- 打开 Fork 后的仓库 → 找到并打开 `auto_login.py`。
- 点击右上角铅笔图标进入编辑模式。
- 替换以下代码：
    
    ```python
    MUSIC_U = "001A18488F6A9E20389EED4442ACBD340B4D4CB03372942A5A8E493059F09F9A19FA8A2686DD62FC9264BE14BCDA66BB835948C058BA3F5D229FECE2507FE2FE32331205A11EA0CF6A67CDDB5601A5035753A7BF5E11A631F3B27FCD8ACE6249FC83B5280619ACEAFD010116B712EC7576578E78DEACE25E9F11013FA0074EF8DCE2152CC7975B617E60928D8A171780F0411FC547FE312C9C241ED49E5E7CA25BC8BE778FCDDAFD984D0D051F1880DAD92FABA1A5C41FD0F438ED5555A658B1B3E998208F0C2F53EF785F95D798CF0EF09F644D8D7B13647CEB958B894753B272C8DF41F5E9C456094BD778390F1E36BF5FC475A58B3D77412BA1639267330C16EE9E7C4718B0A569C43A4A166029FA5E4029CD37B0C06214881888A7A9779D5080F73D59CCDEB592311E97EE7FC1BC71319528073EB6AAF74B6519163A18F34D3EC1CDA16420E2D5501D1E02F1DB4ACD0842A4AB53515D87163010169B2C9898"
    ```
    
- 填好后，点击 **Commit changes** 保存。

### 4. 启动 GitHub Actions

- 进入仓库顶部的 **Actions**。
- 首次使用，点击「I understand my workflows...」启用。
- 选择左侧 `Unlock-NetEaseMusic`，点击右侧 **Run workflow**。
- 运行成功后，自动进入每天定时执行，无需再管。

---

## 🔧 工作原理

1. `NetEaseMusicWorld+` 插件伪装 IP，网易云识别为国内用户。
2. GitHub Actions 每天定时运行，保持 `MUSIC_U` 有效状态。
3. 解锁网易云账号，灰色歌曲正常播放。

---

## ❓ FAQ

### GitHub Actions 首次运行较慢？

首次拉取环境和依赖，属于正常现象。后续自动运行，速度正常。

### 歌曲再次变灰？

`MUSIC_U` 已失效。重新获取 Cookie，重复第 2、3、4 步。

---

## 💡 Issues

有问题请 → [Issues](https://github.com/aoshendev/Unlock-NetEaseMusic-II/issues) ｜ 欢迎 Contribute 👏
