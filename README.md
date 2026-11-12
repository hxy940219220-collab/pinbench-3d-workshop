# Pinbench · 开发板 3D 工坊

Pinbench 是一个基于 Three.js 的开源嵌入式硬件工坊。你可以在浏览器里拆解 3D 开发板、模拟组装焊接，再接上外设运行电路。器材库包含 14 块开发板和 56 个外设模块。

创建人：**Huang Xiyuan** · **且曼学院**

[打开在线工坊](https://pinbench-3d-workshop.vercel.app)

[![Pinbench 3D 展台里的树莓派 4B 爆炸图，接口、芯片和排针分层悬浮在电路板上方](docs/images/pinbench-showcase.webp)](https://pinbench-3d-workshop.vercel.app)

**拆开看元件。** 在展台选择开发板，打开「爆炸图」，旋转模型观察芯片、接口和排针分别装在哪里。器材按系列和用途分组，也可以用键盘选择。

## 从组装到接线

### 组装 Arduino Uno

点击「动手组装」，跟随零件清单摆放芯片和接口。焊接演示会展示烙铁如何接触焊盘，以及焊点如何形成。

![Arduino Uno 组装界面，左侧托盘放着待装元件，烙铁正在接触电路板背面的焊盘](docs/images/pinbench-soldering.webp)

### 运行电路并观察信号

打开「工作台」，从「让 LED 闪起来」入手。按引脚提示接好杜邦线，点击「运行」，观察 LED 和导线上的信号脉冲。在「旋钮调光」任务中，还可以调节电位器，观察 LED 亮度随之改变。工作台也支持自由搭建和传感器仿真。

![旋钮调光任务中，Arduino Uno 通过杜邦线连接电位器和 LED 模块，导线上的光点显示信号活动](docs/images/pinbench-circuit.webp)

导线脉冲反映页面仿真状态，动画速度经过调整以便观察。

## 本地运行

应用代码、模型、样式与数据保存在单文件 `index.html` 中。直接用现代浏览器打开该文件，或在仓库目录启动本地服务。

```sh
python3 -m http.server 8080
```

然后访问 `http://localhost:8080`。页面需要 WebGL，并从 jsDelivr 加载固定版本的 Three.js。

## 部署

这是无需构建的静态站点。Vercel 使用仓库根目录，Framework Preset 选择 Other。

## 开源许可

本项目采用 [MIT 许可证](LICENSE) 开源。Copyright (c) 2026 Huang Xiyuan。
