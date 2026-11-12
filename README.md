# Pinbench · 开发板 3D 工坊

一个基于 Three.js 的嵌入式硬件交互演示工作台。应用代码、模型、样式与数据保存在单文件 `index.html` 中。

- 14 块开发板、56 个外设模块。
- 3D 展台、分层爆炸图、组装与焊接动画。
- 杜邦线连接、课程仿真、信号脉冲与传感器反馈。
- 向上展开的器材分类面板，支持分组、滚动与键盘操作。

## 本地运行

直接用现代浏览器打开 `index.html`，或在此目录运行：

```sh
python3 -m http.server 8080
```

然后访问 `http://localhost:8080`。页面需要 WebGL，并从 jsDelivr 加载固定版本的 Three.js。

## 部署

这是无需构建的静态站点。Vercel 使用仓库根目录，Framework Preset 选择 Other。

导线脉冲反映页面仿真状态，并为教学展示进行了时间放大。
