# tvbox-source

影视仓 / TVBox 整合多仓配置（明老板家用，2026-08-28 实测）。

## 用法（影视仓）

1. 打开影视仓 → 设置 → **配置地址** → 添加
2. 粘贴（首选）：
   ```
   https://gh-proxy.com/https://raw.githubusercontent.com/hejm2000/tvbox-source/main/tvbox.json
   ```
   备选（gh-proxy 挂掉时换）：
   ```
   https://raw.githubusercontent.com/hejm2000/tvbox-source/main/tvbox.json
   ```
3. 保存后影视仓会自动拉取，首页出现 8 条线路，可任意切换。

> 本仓库为公共仓库（内容只有配置链接，无敏感信息），raw 直链匿名可访问。

## 内置线路（导入时均实测可达）

| # | 线路 | 说明 | 实测 |
|---|------|------|------|
| 1 | noimank 多仓合集 | 14 条线路一次全有 | gitlab 0.8s |
| 2 | noimank 健康家用 | 64 源 + 直播，spider 685KB 首载需等 | 3s |
| 3 | FongMI 0827 | 33 源，老牌稳定 | gh-proxy |
| 4 | 高天流云 js | drpy 版，备用 | gh-proxy |
| 5 | 小盒子 4K | 4K 向 | 0.8s |
| 6 | 香雅情 XYQ | XYQ 源 | gh-proxy |
| 7 | felixiao 18+ | 35 个 18+ 源（91麻豆/色猫/CK/皇冠等） | raw 5.7s |
| 8 | scovis R18 | 101 源大合集，实测存活约 4-18 个 | gh-proxy |

## 维护

- 某条线路失效：改 `tvbox.json` 对应条目 → commit → push，电视上重新拉一次配置即可。
- 18+ 源死亡率高属正常，隔段时间换批。
- 所有源均为网络收集，仅供自用。
