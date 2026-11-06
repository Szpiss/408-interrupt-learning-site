# 408 中断与异常 · 交互学习站

面向考研 408 的中断与异常交互学习页面，串联计算机组成原理与操作系统中的相关知识点。

## 在线学习

[直接打开学习站](https://szpiss.github.io/408-interrupt-learning-site/)，无需下载或登录 GitHub。

## 下载与使用

1. 点击仓库页面的 **Code → Download ZIP**，或[直接下载 ZIP](https://github.com/Szpiss/408-interrupt-learning-site/archive/refs/heads/main.zip)。
2. 解压下载的文件。
3. 双击 `index.html`，用 Chrome、Safari 或 Edge 打开。

页面完全离线运行，无需安装 Python、Node.js 或启动服务器。也可以只下载仓库中的 `index.html` 文件使用。

## 主要功能

- 8 大知识模块，覆盖中断、异常、进程调度、缺页、I/O 与 DMA 等内容。
- 中断响应流程实验与中断嵌套判断。
- 知识章节、易错提醒及章节笔记。
- 20 道综合自测题，支持按章节练习、自动评分和讲解。
- 错题本、学习进度记录和全文搜索。
- 通过浏览器打印功能保存为 PDF。

## 学习记录

进度、笔记和错题保存在当前浏览器的 `localStorage` 中，不会自动跨浏览器或设备同步。部分浏览器可能限制本地文件页面的存储；清除浏览器数据也可能导致记录丢失。

## 内容说明

内容以 408 的经典模型和考查范围为主；不同 CPU 架构的具体行为可能不同，以考试教材和题目约定为准。页面对 2021 年“进入中断响应周期时 CPU 开中断”的表述标注了教材判题语境与严格解释之间的歧义。

更多说明见 [README.txt](README.txt)。


## 网站访问统计

线上版本使用免费的Cloudflare Web Analytics，网站仍部署在GitHub Pages。进入自己的Cloudflare账号，在Observability → Analytics → Web analytics中选择`szpiss.github.io`查看。用Path筛选对应站点：

- 中断站：`/408-interrupt-learning-site/`（或`/408-interrupt-learning-site/index.html`）。
- 信号量站：`/408-semaphore-learning-site/`（或`/408-semaphore-learning-site/index.html`）。

本次只统计完整页面加载，不把章节切换、翻卡片或每次答题重复计为一次页面浏览。数据从接入后开始，不能补回历史访问；Cloudflare的Visits是服务自身定义的访问指标，并非精确去重人数。界面通常有数分钟延迟，浏览器拦截或网络异常可造成漏计。

脚本仅在`https://szpiss.github.io`的两个指定站点路径加载，file://、本地预览及其他域名均不加载。尊重浏览器Do Not Track与Global Privacy Control。网站不上传本机的学习进度、笔记、答题或错题内容。

全部学习功能仍可离线运行；Cloudflare脚本不是学习功能的运行依赖。网页里的Cloudflare站点标识是公开的统计配置，不是账户API密钥。请勿把Cloudflare账户API密钥或登录信息提交到仓库。

维护时请保留线上加载条件；如果调整信号量站的Content Security Policy，必须继续允许官方统计脚本地址和官方数据接收端点。
