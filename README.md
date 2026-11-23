# 彩虹跑马灯边界线

这是一个 CC GUI Tier-0 声明式插件，在对话运行（AI 生成/回复）期间为整个聊天输入框显示 2px 的彩虹渐变边界线，颜色会沿边界持续循环流动；空闲时自动恢复常规边框。

插件不申请额外权限，也不包含 JavaScript。

## 特性

- 🌈 **动态触发**：仅在当前对话运行中（AI 正在生成回复）展示流动彩虹跑马灯，空闲状态无侵入恢复原生边框。
- ⚡ **零 JS 开销**：Tier-0 声明式设计，纯 GPU 加速 CSS 动画，无额外运行时消耗。
- 🔒 **纯安全**：0 权限申请，无网络请求，无脚本审计负担。

## 安装

在 CC GUI 应用内的插件市场搜索「彩虹跑马灯边界线」一键安装。

## 手动安装（本地开发）

把整个文件夹放到 CC GUI 的本地插件目录（`设置 → 插件 → 打开插件目录`），重载即可。

## 发版

```bash
git tag 1.1.0 && git push origin 1.1.0
```

推送与 `manifest.json` 的 `version` 完全一致的 tag（无 `v` 前缀）后，GitHub Action 会自动把
`manifest.json` / `styles.css` / `checksums.txt` 附加到该 tag 的 Release。

## License

[MIT](LICENSE)
