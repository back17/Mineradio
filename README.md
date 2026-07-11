[README.md](https://github.com/user-attachments/files/29926405/README.md)
# Mineradio Weather Edition

`back17` 的非官方天气增强二创版。

Mineradio Weather Edition 把天气从背景信息变成首页的主入口：打开应用就能看到当前城市、短时预报和未来趋势；点进面板后可以直接切换城市，查看更完整的天气变化，再按当下天气开启对应氛围的音乐队列。

> 本项目基于 [XxHuberrr/Mineradio](https://github.com/XxHuberrr/Mineradio) 二次开发，与原项目及任何音乐平台均无官方关联。完整改动记录见 [MODIFICATIONS.md](./MODIFICATIONS.md)。

## 这次二创做了什么

- 将 Home 左侧的施工占位区域改造成完整天气预报面板。
- 保留原有暗色玻璃、紧凑信息密度和 Home 视觉语言，不把天气做成突兀的外来组件。
- 点击天气面板即可进入详情页，查看 8 项实时指标、未来 24 小时和未来 7 天预报。
- 支持输入城市切换、网络定位、刷新天气和一键开启天气电台。
- 扩展 Open-Meteo 数据：气压、能见度、阵风、降水总量、日出日落和 UV 指数。
- Home 首页保持 6 小时 / 4 天的精简视图，详情页再展开完整信息，避免首页被塞满。

## 当前版本

- 二创维护者：`back17`
- 修改版版本：`1.1.1-weather.1`
- 上游基线：`Mineradio v1.1.1`
- 发布页：[back17/Mineradio Releases](https://github.com/back17/Mineradio/releases)

Release 资产生成后，请从本仓库的 Releases 下载对应安装包；不要混用上游仓库的安装包与本修改版。

## 运行与构建

```powershell
npm ci
npm start
```

构建 Windows 安装包：

```powershell
npm run build:win
```

构建产物会写入 `dist/`。发布时建议上传：

- `Mineradio-1.1.1-weather.1-Setup.exe`
- `Mineradio-1.1.1-weather.1-Setup.exe.blockmap`
- `latest.yml`
- 安装包的 SHA256 校验文件

## 天气与音乐

天气信息由 Open-Meteo 提供。天气电台会依据当前天气、时间和城市生成音乐搜索词与播放队列；它是本地播放器体验的一部分，不会替代或绕过任何音乐平台的会员、版权或播放权限。

## 隐私与第三方服务

登录 Cookie、搜索历史、自定义封面、自定义歌词和节奏分析缓存仅应保留在本机，不应提交到仓库。网易云音乐、QQ 音乐及其他第三方服务均有各自的服务条款与版权规则，请使用自己的账号并遵守相应规则。

更多隐私说明见 [PRIVACY.md](./PRIVACY.md)。

## 来源与授权

本项目的上游代码来自 [XxHuberrr/Mineradio](https://github.com/XxHuberrr/Mineradio)，上游提交基线为 `6b130103f759e5dcd1e133700071c8216b8fa5a6`。

原项目版权归 XxHuberrr 所有。本二创版本继续以 GPL-3.0 发布，保留原始 [LICENSE](./LICENSE) 与 [NOTICE.md](./NOTICE.md)，并在 [MODIFICATIONS.md](./MODIFICATIONS.md) 中明确记录改动。

`Mineradio` 名称、MR Logo、原始界面视觉表达及其他原作者保留权利不因本仓库的 GPL 代码授权而自动转让。
