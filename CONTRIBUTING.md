# 贡献指南

感谢你对 Obsidian Markdown Visualizer 插件的关注！

## 🤝 如何贡献

### 报告 Bug

如果你发现了 bug，请：

1. 检查 [Issues](https://github.com/wangjia15/obsidian-markdown-visualizer/issues) 是否已有相关报告
2. 如果没有，创建新的 Issue，包含：
   - 清晰的标题和描述
   - 重现步骤
   - 预期行为 vs 实际行为
   - 截图（如果适用）
   - Obsidian 版本和插件版本

### 建议新功能

欢迎提出新功能建议：

1. 在 [Issues](https://github.com/wangjia15/obsidian-markdown-visualizer/issues) 中创建功能请求
2. 详细描述功能需求和使用场景
3. 如果可能，提供示例或参考

### 提交 Pull Request

1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交改动 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

### 代码规范

- 使用 TypeScript 类型注解
- 遵循现有代码风格
- 添加必要的注释
- 确保代码通过测试

### 新增 Infographic 模板

如果你想添加新的 Infographic 模板：

1. 在 `main.js` 中添加 `render[TemplateName]()` 方法
2. 在 `styles.css` 中添加对应样式
3. 在 `renderInfographic()` 中添加路由逻辑
4. 创建测试示例
5. 更新 README 文档

## 📝 开发设置

### 环境要求

- Node.js 14+
- Obsidian 1.0.0+

### 本地开发

1. Clone 仓库
```bash
git clone https://github.com/wangjia15/obsidian-markdown-visualizer.git
```

2. 复制插件文件到 Obsidian 插件目录
```bash
cp -r .obsidian/plugins/markdown-visualizer ~/.obsidian/plugins/
```

3. 在 Obsidian 中启用插件

4. 修改代码后重新加载 Obsidian (`Ctrl + R`)

## 🧪 测试

使用提供的测试文件验证功能：

- `插件测试.md` - 基础功能测试
- `新模板测试.md` - 新模板测试

## 📜 许可证

通过贡献，你同意你的贡献将在 MIT 许可证下授权。

## 💬 社区

- GitHub Issues: 报告问题和建议
- GitHub Discussions: 讨论和交流

---

再次感谢你的贡献！🎉
