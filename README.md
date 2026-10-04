<div align="center">
  <img src="https://scanops.niigel.com/logo.svg" alt="ScanOps" width="96" height="96" />

  # ScanOps Browser SDK

  **中文** | [English](README.en.md)

  [🔗 在线体验](https://scanops.niigel.com) · [📖 完整开发文档](https://scanops.niigel.com/zh-Hans/docs)
</div>

**给你的 Web 应用装上一双能识码的眼睛。** 无需下载 App、无需跳转小程序，浏览器里几行代码即可调起摄像头，识别二维码与主流一维条码——解码全程在用户设备本地完成，画面不上传、不经云端。

- **快而不卡顿** —— 识别运行在独立 Web Worker 线程，不阻塞页面交互，收银台、拣货枪也能流畅响应
- **准而不误触发** —— 内置多帧确认与轨迹追踪，同一个码不会被重复计数，专为高频扫描场景打磨
- **十种码制开箱即用** —— QRCode、Code128、Code39、Code93、EAN13、EAN8、UPC-A、UPC-E、ITF、Codabar
- **框架无关** —— 原生 TypeScript / ESM，H5 与 Vue 直接调用 `ScanOps`，React 项目可直接使用 `ScanOpsView` 组件
- **按客户授权下发** —— 核心定位模型专属加密下发，只在你登记过的域名上运行，保障商业授权可控

npm 包：[`@niigelog/scanops`](https://www.npmjs.com/package/@niigelog/scanops)

## 开始使用

安装、部署运行文件、原生与 React 的接入示例、参数和事件说明，都在开发文档里：

👉 **[ScanOps 开发文档](https://scanops.niigel.com/zh-Hans/docs)**

接入前请先了解：

- **需要 license key** —— 按域名签发，只在登记过的域名（含本地开发地址）上生效。未授权时摄像头仍可预览，但不识别。
- **需要 HTTPS 或 localhost** —— 浏览器只在安全上下文中开放摄像头。
- **仅提供 ESM 入口** —— React 组件需要 React 18.2 或 19。

