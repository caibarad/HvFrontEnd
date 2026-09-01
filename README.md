# HvGuard VT 调试器

基于 Intel VT-x 的虚拟化调试 / 反调试对抗框架。

## 支持平台

- Intel Xeon E5
- Intel Core i5 / i7 / i9（任意代）
- Intel Core Ultra（Arrow Lake） - 已经发布1.0

## 开发计划

- [ ] 调试器相关问题修复
- [ ] 考虑支持 AMD（SVM / NPT）

用法:
【VT工具 调试程序】 https://www.bilibili.com/video/BV1hp846TEJj/?share_source=copy_web&vd_source=c5e653091a2a2569e262bc474e614b4c

## 修复记录 - 8.30

**问题**：在NP盾 保护中 同时开 CE 和 DBG 两个调试器时，只有一个能正常工作（调试器覆盖问题）
CE 调试完成 脱离 ，DBG 无法调试  ，已经修复相关问题。

## 修复记录 - 9.1

**问题**：在调试相关程序时 程序会下WH_MOUSE_LL 钩子 导致下段 鼠标卡住 已经修复相关问题。

！调试器软件不再更新
