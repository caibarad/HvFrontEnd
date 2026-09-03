# HvGuard VT 调试器

> [!WARNING]  
> **本项目已停止更新，调试器软件不再维护。**  
> 最后修复记录：9.1

基于 Intel VT-x 的虚拟化调试 / 反调试对抗框架。

## 支持平台

- Intel Xeon E5
- Intel Core i5 / i7 / i9（任意代）
- Intel Core Ultra（Arrow Lake） - 已经发布1.0

## 开发计划

- [ ] 调试器相关问题修复
- [ ] 考虑支持 AMD（SVM / NPT）

> 注：因项目不再更新，上述计划可能不会继续实现。

## 用法

【VT工具 调试程序】 https://www.bilibili.com/video/BV1hp846TEJj/?share_source=copy_web&vd_source=c5e653091a2a2569e262bc474e614b4c

## 修复记录

### 8.30
**问题**：在 NP 盾保护中同时开 CE 和 DBG 两个调试器时，只有一个能正常工作（调试器覆盖问题）。  
CE 调试完成脱离后，DBG 无法调试。已修复相关问题。

### 9.1
**问题**：在调试相关程序时，程序会下 `WH_MOUSE_LL` 钩子导致下断后鼠标卡住。已修复相关问题。

## 9.3
**问题**：在接管调试之后 运行调试器之后 打开EAC 导致蓝屏 ，以及EAC 64 检测硬断 断点问题 。已修复相关问题。
## 停止更新说明

本调试器软件不再更新，后续问题请自行处理
