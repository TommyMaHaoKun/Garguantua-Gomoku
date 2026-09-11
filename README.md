# Garguantua Gomoku

**Gargantua 1.1 online · Author: Haokun Ma**

在线五子棋 AI 的 Windows 发行仓库。1.1 online 客户端**不含模型权重**,对弈由作者
托管的在线推理服务完成——客户端只发送棋局、接收落子。运行需要联网。

## 下载与运行

从 [最新发行版](https://github.com/TommyMaHaoKun/Garguantua-Gomoku/releases/latest)
下载 `Gargantua 1.1 online.exe`,双击运行。

- Windows 10 / 11,64 位 x64;无需安装 Python,也无需账号。
- **需要联网**:AI 由在线服务计算。首次连接若服务器休眠,会自动等待其唤醒(约 10–20 秒)。
- 可选 9×9、13×13、15×15、19×19 棋盘。
- 胜负显示在侧边栏,棋盘始终完整可见。

U / Backspace:悔棋;R / Enter:重开;C:切换执子;S:显示评分。
更多信息见 [使用说明](README.txt) 与 [版权声明](NOTICE.txt)。

### 指定服务器(可选)

客户端默认连接内置地址。也可用环境变量临时覆盖后再启动:

```
set GARGANTUA_SERVER=https://你的服务地址
```

## 为什么是"在线"

离线发行版会把模型打包进 EXE,权重可从进程/文件中被提取。1.1 online 把模型放在
作者控制的服务器上,**权重不随客户端分发**,这是真正防止权重被提取的形态。

## 版本

- **1.1 online**(当前):在线客户端,无本地权重。
- **V1.0 离线**:见 [`offline-v1.0/`](offline-v1.0/) 目录(说明与预览);安装包见对应发行版。

---

NO PLAGIARISM. This client ships no model weights; play is served by the author's
hosted inference service. Do not extract or redistribute weights, or claim the
original model or code as your own. See [NOTICE.txt](NOTICE.txt).
